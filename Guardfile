require 'guard/guard'

guard :rspec, :all_on_start => false, :all_after_pass => false, :cli => '--fail-fast --format doc' do
  watch(%r{^spec/.+_spec\.rb$})
  watch(%r{^lib/(.+)\.rb$})                { |m| "spec/#{m[1]}_spec.rb" }
  watch('spec/spec_helper.rb')             { "spec" }
end
