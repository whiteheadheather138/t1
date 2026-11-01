代发 wailian999

Py:   resp.json()
来源：http://m.share.tarul.cn/Article/details/ggvkctdgw.sHtML

PHP:  json_decode($body, true);
来源：http://read.share.epnwcf.com/Article/details/gfpkxzrof.sHtML

JS:   await resp.json()
来源：http://blog.sjlbkw.cn/Article/details/gwvktmvlq.sHtML

TS:   await resp.json()
来源：http://mobile.fktsv.cn/Article/details/guvypjfpo.sHtML

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baike.bbcook.cn/Article/details/gjljsozvn.sHtML

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://www.share.fktsv.cn/Article/details/gqceoqoln.sHtML

Ruby: JSON.parse(resp.body)
来源：http://www.share.yfazqb.com/Article/details/ggxjgzfkj.sHtML

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wap.tarul.cn/Article/details/gmsrmgqgn.sHtML

[L07] 处理 HTTP 状态码
来源：http://read.share.sjlbkw.cn/Article/details/gvsqhwxnp.sHtML

Py:   resp.status_code;  resp.raise_for_status()
来源：http://read.share.epnwcf.com/Article/details/ghlnbxkta.sHtML

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mobile.sjlbkw.cn/Article/details/gjwfebaos.sHtML

JS:   resp.ok;  resp.status
来源：http://mobile.vehdjk.com/Article/details/grhobewdc.sHtML

TS:   resp.ok;  resp.status
来源：http://m.share.vehdjk.com/Article/details/gveezipgq.sHtML

Java: resp.statusCode()
来源：http://mobile.bbcook.cn/Article/details/ggxkrhfsp.sHtML

Go:   resp.StatusCode
来源：http://www.blog.bbcook.cn/Article/details/gtccmayrq.sHtML

Ruby: resp.code.to_i
来源：http://www.share.tarul.cn/Article/details/gkohykbae.sHtML

C#:   (int)resp.StatusCode
来源：http://wap.epnwcf.com/Article/details/gynooynkb.sHtML

[L08] 并发请求多个地址
来源：http://www.blog.sjlbkw.cn/Article/details/gjfexbmvo.sHtML

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://www.m.share.yfazqb.com/Article/details/gsotepzfa.sHtML

PHP:  curl_multi_init() 系列
来源：http://blog.epnwcf.com/Article/details/gymgzifcd.sHtML

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://www.blog.yfazqb.com/Article/details/gwhnucbhl.sHtML

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://read.share.bbcook.cn/Article/details/giuncdtzy.sHtML

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wap.vehdjk.com/Article/details/gzhsphayg.sHtML

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://www.blog.bbcook.cn/Article/details/gubewctem.sHtML

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://baike.bbcook.cn/Article/details/gaabvjjnv.sHtML

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://www.blog.tarul.cn/Article/details/gksgdwijn.sHtML

================================================================================
来源：http://read.share.bbcook.cn/Article/details/gurlzuzfr.sHtML

M. 命令行 / 进程 / 环境
来源：http://www.m.share.yfazqb.com/Article/details/guhsfkrdg.sHtML

================================================================================
来源：http://www.share.epnwcf.com/Article/details/grxgknlwf.sHtML

[M01] 读取命令行参数
来源：http://3g.tarul.cn/Article/details/gspmppbzg.sHtML

Py:   sys.argv[1:]
来源：http://read.share.sjlbkw.cn/Article/details/gtmjdcciy.sHtML

PHP:  $argv;  $argc;
来源：http://www.share.tarul.cn/Article/details/gatbupeeb.sHtML

JS:   process.argv.slice(2)
来源：http://www.share.epnwcf.com/Article/details/gryfahpge.sHtML

TS:   process.argv.slice(2)
来源：http://baike.bbcook.cn/Article/details/ghipbuhdz.sHtML

Java: args 数组（main 方法参数）
来源：http://www.blog.bbcook.cn/Article/details/geblcbvsc.sHtML

Go:   os.Args[1:]
来源：http://mobile.tarul.cn/Article/details/glloktfoy.sHtML

Ruby: ARGV
来源：http://m.share.fktsv.cn/Article/details/gkubvjcqf.sHtML

C#:   args 数组（Main 方法参数）
来源：http://read.share.fktsv.cn/Article/details/grovfsrqs.sHtML

[M02] 读取环境变量
来源：http://3g.tarul.cn/Article/details/govqknwhv.sHtML

Py:   os.environ.get("HOME")
来源：http://3g.epnwcf.com/Article/details/guespilns.sHtML

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://blog.vehdjk.com/Article/details/gjvdlilyq.sHtML

JS:   process.env.HOME
来源：http://wap.bbcook.cn/Article/details/gjbloctzr.sHtML

TS:   process.env.HOME
来源：http://m.share.epnwcf.com/Article/details/gehboammv.sHtML

Java: System.getenv("HOME")
来源：http://wap.yfazqb.com/Article/details/gpvrkbspb.sHtML

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://baike.vehdjk.com/Article/details/gaekktoyb.sHtML

Ruby: ENV["HOME"]
来源：http://wap.sjlbkw.cn/Article/details/gbnoyowvu.sHtML

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://read.share.tarul.cn/Article/details/gcaxviall.sHtML

[M03] 执行外部命令
来源：http://3g.fktsv.cn/Article/details/guybqnfdl.sHtML

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mobile.epnwcf.com/Article/details/gxgkrfaeh.sHtML

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://baike.yfazqb.com/Article/details/gkicjhsvz.sHtML

JS:   child_process.execSync("ls -l").toString()
来源：http://baike.sjlbkw.cn/Article/details/goqqzbose.sHtML

TS:   child_process.execSync("ls -l").toString()
来源：http://www.blog.bbcook.cn/Article/details/gkzjinxap.sHtML

Java: new ProcessBuilder("ls", "-l").start()
来源：http://read.share.bbcook.cn/Article/details/gtmhbsndm.sHtML

Go:   exec.Command("ls", "-l").Output()
来源：http://m.share.vehdjk.com/Article/details/gfisybiwy.sHtML

Ruby: system("ls -l");  `ls -l`
来源：http://wap.vehdjk.com/Article/details/gmsnnpdqy.sHtML

C#:   Process.Start("ls", "-l");
来源：http://mobile.epnwcf.com/Article/details/gmjyxfafp.sHtML

[M04] 获取当前工作目录
来源：http://3g.yfazqb.com/Article/details/gxiapkfuf.sHtML

Py:   os.getcwd()
来源：http://read.share.yfazqb.com/Article/details/gebozdhor.sHtML

PHP:  getcwd();
来源：http://3g.fktsv.cn/Article/details/gdlaelsab.sHtML

JS:   process.cwd()
来源：http://read.share.tarul.cn/Article/details/ghkckfxer.sHtML

TS:   process.cwd()
来源：http://blog.sjlbkw.cn/Article/details/gaapzegtb.sHtML

Java: Path.of("").toAbsolutePath()
来源：http://wap.tarul.cn/Article/details/gsxuoahrk.sHtML

Go:   os.Getwd()
来源：http://baike.tarul.cn/Article/details/gifgnldjr.sHtML

Ruby: Dir.pwd
来源：http://3g.fktsv.cn/Article/details/gghffvsct.sHtML

C#:   Directory.GetCurrentDirectory()
来源：http://mobile.tarul.cn/Article/details/gfyklobfo.sHtML

[M05] 设置退出码
来源：http://www.blog.yfazqb.com/Article/details/goupdoadu.sHtML

Py:   sys.exit(1)
来源：http://www.m.share.sjlbkw.cn/Article/details/gitqhqmtl.sHtML

PHP:  exit(1);
来源：http://baike.bbcook.cn/Article/details/gghifvmgc.sHtML

JS:   process.exit(1)
来源：http://www.m.share.tarul.cn/Article/details/gcndlmijy.sHtML

TS:   process.exit(1)
来源：http://www.m.share.bbcook.cn/Article/details/gbkelrmyh.sHtML

Java: System.exit(1)
来源：http://www.share.sjlbkw.cn/Article/details/gosathxqb.sHtML

Go:   os.Exit(1)
来源：http://www.m.share.vehdjk.com/Article/details/gzfeczokk.sHtML

Ruby: exit 1
来源：http://mobile.sjlbkw.cn/Article/details/gmdysuopp.sHtML

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://baike.bbcook.cn/Article/details/gsirvongq.sHtML

[M06] 向标准错误输出
来源：http://blog.tarul.cn/Article/details/gpnntttwz.sHtML

Py:   print("err", file=sys.stderr)
来源：http://www.m.share.yfazqb.com/Article/details/gfxsddhjh.sHtML

PHP:  fwrite(STDERR, "err\n");
来源：http://www.m.share.bbcook.cn/Article/details/ghmbwylnh.sHtML

JS:   console.error("err")
来源：http://read.share.fktsv.cn/Article/details/glepsgzcp.sHtML

TS:   console.error("err")
来源：http://m.share.bbcook.cn/Article/details/gqcizokym.sHtML

Java: System.err.println("err")
来源：http://www.m.share.sjlbkw.cn/Article/details/gpwjasfsv.sHtML

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://www.share.fktsv.cn/Article/details/gfqkvccqz.sHtML

Ruby: warn "err"
来源：http://www.share.bbcook.cn/Article/details/gtspjihsb.sHtML

C#:   Console.Error.WriteLine("err")
来源：http://wap.sjlbkw.cn/Article/details/gzqikaaid.sHtML

[M07] 判断是否为主入口
来源：http://mobile.bbcook.cn/Article/details/gecoxrwnv.sHtML

Py:   if __name__ == "__main__":
来源：http://wap.tarul.cn/Article/details/gcrdijgak.sHtML

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://3g.vehdjk.com/Article/details/grwopjurz.sHtML

JS:   require.main === module
来源：http://www.blog.bbcook.cn/Article/details/gtctiiluq.sHtML

TS:   require.main === module
来源：http://www.m.share.sjlbkw.cn/Article/details/gnwctwsnz.sHtML

Java: public static void main(String[] args)
来源：http://m.share.fktsv.cn/Article/details/gsyjqrsiq.sHtML

Go:   func main()
来源：http://www.share.bbcook.cn/Article/details/gfsvgnizw.sHtML

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://www.m.share.yfazqb.com/Article/details/gyhjjojan.sHtML

C#:   static void Main(string[] args)
来源：http://m.share.tarul.cn/Article/details/gemdslrwf.sHtML

[M08] 获取系统与运行时信息
来源：http://www.blog.tarul.cn/Article/details/gvbbuovcf.sHtML

Py:   platform.system();  platform.python_version()
来源：http://m.share.yfazqb.com/Article/details/gvyszmulg.sHtML

PHP:  PHP_OS;  phpversion();
来源：http://www.m.share.sjlbkw.cn/Article/details/gxvaqesfx.sHtML

JS:   process.platform;  process.version
来源：http://www.share.epnwcf.com/Article/details/gfinfykie.sHtML

TS:   process.platform;  process.version
来源：http://blog.bbcook.cn/Article/details/gazjqdzqv.sHtML

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://3g.bbcook.cn/Article/details/gqtvtrdcq.sHtML

Go:   runtime.GOOS;  runtime.Version()
来源：http://read.share.sjlbkw.cn/Article/details/gmshzfpne.sHtML

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://www.share.sjlbkw.cn/Article/details/gqsbfpvis.sHtML

C#:   Environment.OSVersion;  Environment.Version
来源：http://blog.epnwcf.com/Article/details/gbhfyrwkq.sHtML

================================================================================
来源：http://www.m.share.yfazqb.com/Article/details/gdleacxmf.sHtML

N. 数据结构与算法
来源：http://www.share.tarul.cn/Article/details/gdfjcvxod.sHtML

================================================================================
来源：http://3g.vehdjk.com/Article/details/glclibuoy.sHtML

[N01] 二分查找（有序数组）
来源：http://m.share.tarul.cn/Article/details/gmuhilgtq.sHtML

Py:   bisect.bisect_left(arr, x)
来源：http://www.blog.sjlbkw.cn/Article/details/gyouxnhlh.sHtML

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://blog.yfazqb.com/Article/details/gwfezcrlr.sHtML

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://www.m.share.vehdjk.com/Article/details/gaazhdcwb.sHtML

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://blog.sjlbkw.cn/Article/details/gpbukwmkw.sHtML

Java: Arrays.binarySearch(arr, x)
来源：http://www.m.share.sjlbkw.cn/Article/details/gwczvnqcg.sHtML

Go:   sort.SearchInts(arr, x)
来源：http://3g.tarul.cn/Article/details/gkwevzlrg.sHtML

Ruby: arr.bsearch { |e| e >= x }
来源：http://baike.vehdjk.com/Article/details/gzxlzxnci.sHtML

C#:   Array.BinarySearch(arr, x)
来源：http://m.share.sjlbkw.cn/Article/details/giwamzbdl.sHtML

[N02] 排序（工程实践用内置实现）
来源：http://wap.sjlbkw.cn/Article/details/glachdraz.sHtML

Py:   sorted(arr);  arr.sort()
来源：http://m.share.yfazqb.com/Article/details/gyiakbizv.sHtML

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://wap.yfazqb.com/Article/details/gxiqxjauc.sHtML

JS:   [...arr].sort((a, b) => a - b)
来源：http://mobile.tarul.cn/Article/details/ganzxvkfu.sHtML

TS:   [...arr].sort((a, b) => a - b)
来源：http://m.share.vehdjk.com/Article/details/gsjsmregu.sHtML

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://www.blog.vehdjk.com/Article/details/gajixkfgb.sHtML

Go:   slices.Sort(arr)
来源：http://baike.epnwcf.com/Article/details/gkvwvkcoz.sHtML

Ruby: arr.sort
来源：http://read.share.tarul.cn/Article/details/goakffpxe.sHtML

C#:   Array.Sort(arr);  list.Sort()
来源：http://www.m.share.epnwcf.com/Article/details/gnxmuhsfq.sHtML

[N03] 快速排序（分治示例）
来源：http://www.share.yfazqb.com/Article/details/gzwbmddtm.sHtML

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://www.m.share.sjlbkw.cn/Article/details/gifpouctc.sHtML

PHP:  // 递归实现，或用 usort
来源：http://www.share.tarul.cn/Article/details/gfwulwaqv.sHtML

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://blog.fktsv.cn/Article/details/gtydydfbm.sHtML

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mobile.bbcook.cn/Article/details/gisoxdgdy.sHtML

Java: // 手写递归，或直接用 Arrays.sort
来源：http://www.m.share.fktsv.cn/Article/details/gdfqwnrnf.sHtML

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://blog.vehdjk.com/Article/details/gqxqgfytp.sHtML

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://3g.yfazqb.com/Article/details/gypwifogb.sHtML

C#:   // 手写递归，或 Array.Sort
来源：http://www.share.tarul.cn/Article/details/gdxbvyvbs.sHtML

[N04] 斐波那契数列
来源：http://baike.sjlbkw.cn/Article/details/gqdvwmxgu.sHtML

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://www.share.epnwcf.com/Article/details/gupjikpiv.sHtML

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://read.share.fktsv.cn/Article/details/gvakckjxl.sHtML

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://www.blog.epnwcf.com/Article/details/gsorvdmcj.sHtML

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://blog.yfazqb.com/Article/details/gqmfqjpwp.sHtML

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blog.fktsv.cn/Article/details/gvjgcivyk.sHtML

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://blog.bbcook.cn/Article/details/glnkxdbww.sHtML

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://wap.epnwcf.com/Article/details/gajvzbclb.sHtML

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://www.share.tarul.cn/Article/details/gjpibpaqz.sHtML

[N05] 最大公约数
来源：http://www.share.epnwcf.com/Article/details/grvgiwnzd.sHtML

Py:   math.gcd(a, b)
来源：http://www.share.fktsv.cn/Article/details/gqxshhtek.sHtML

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://blog.bbcook.cn/Article/details/gmhrudfdm.sHtML

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.bbcook.cn/Article/details/gjdcrxwku.sHtML

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://m.share.tarul.cn/Article/details/givpetsde.sHtML

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://www.m.share.bbcook.cn/Article/details/gpznlsdhq.sHtML

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mobile.bbcook.cn/Article/details/gqxuxdlpq.sHtML

Ruby: a.gcd(b)
来源：http://wap.bbcook.cn/Article/details/galddonvr.sHtML

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://blog.sjlbkw.cn/Article/details/gglizrsia.sHtML

[N06] 判断回文字符串
来源：http://www.blog.yfazqb.com/Article/details/gqaqnfiif.sHtML

Py:   s == s[::-1]
来源：http://m.share.fktsv.cn/Article/details/gdlxzejtl.sHtML

PHP:  $s === strrev($s);
来源：http://m.share.bbcook.cn/Article/details/gltbtxkuk.sHtML

JS:   s === [...s].reverse().join("")
来源：http://3g.epnwcf.com/Article/details/gqigmjqui.sHtML

TS:   s === [...s].reverse().join("")
来源：http://wap.fktsv.cn/Article/details/ggcrjymnr.sHtML

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://www.blog.vehdjk.com/Article/details/gobnwlzyx.sHtML

Go:   // 双指针从两端比较
来源：http://baike.yfazqb.com/Article/details/gtpnufrmz.sHtML

Ruby: s == s.reverse
来源：http://www.m.share.vehdjk.com/Article/details/gwqwopubf.sHtML

C#:   s == new string(s.Reverse().ToArray())
来源：http://wap.fktsv.cn/Article/details/gwzkxvjqx.sHtML

[N07] 两数之和（返回下标）
来源：http://mobile.sjlbkw.cn/Article/details/gmpibofwe.sHtML

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://baike.vehdjk.com/Article/details/gfledjrhe.sHtML

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://m.share.epnwcf.com/Article/details/gocpjexps.sHtML

JS:   // 手写 Map：map.set(v, i)
来源：http://m.share.yfazqb.com/Article/details/gxhnsrcfx.sHtML

TS:   // 手写 Map<string, number>
来源：http://wap.vehdjk.com/Article/details/gbpkufmfd.sHtML

Java: // 手写 HashMap
来源：http://read.share.epnwcf.com/Article/details/gdsevanuv.sHtML

Go:   // 手写 map[int]int
来源：http://www.blog.tarul.cn/Article/details/gyrkqseyj.sHtML

Ruby: // 手写 Hash
来源：http://3g.epnwcf.com/Article/details/goeypohqp.sHtML

C#:   // 手写 Dictionary<int, int>
来源：http://www.m.share.epnwcf.com/Article/details/gwwnqesqo.sHtML

[N08] 生成全排列
来源：http://www.m.share.yfazqb.com/Article/details/gboqovqmw.sHtML

Py:   itertools.permutations(arr)
来源：http://www.share.yfazqb.com/Article/details/gswujowop.sHtML

PHP:  // 手写递归交换
来源：http://3g.tarul.cn/Article/details/gpiexmiqa.sHtML

JS:   // 手写回溯递归
来源：http://mobile.sjlbkw.cn/Article/details/gnzfdhrau.sHtML

TS:   // 手写回溯递归
来源：http://blog.tarul.cn/Article/details/gluaiiqjk.sHtML

Java: // 手写回溯递归
来源：http://www.m.share.epnwcf.com/Article/details/goiryooxo.sHtML

Go:   // 手写回溯递归
来源：http://wap.bbcook.cn/Article/details/gulldfzxy.sHtML

Ruby: arr.permutation.to_a
来源：http://blog.sjlbkw.cn/Article/details/gsjqeshqb.sHtML

C#:   // 手写回溯递归
来源：http://blog.yfazqb.com/Article/details/gxeslwtid.sHtML

[N09] 栈与队列
来源：http://read.share.sjlbkw.cn/Article/details/gjqpcevcs.sHtML

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://www.m.share.bbcook.cn/Article/details/guljxjtnm.sHtML

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://read.share.epnwcf.com/Article/details/gewimzrnc.sHtML

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://m.share.fktsv.cn/Article/details/gwiluddyf.sHtML

TS:   arr.push(x) / arr.pop() 作栈
来源：http://baike.tarul.cn/Article/details/gxyiuwqfk.sHtML

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://mobile.fktsv.cn/Article/details/ghqjssddo.sHtML

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://www.share.fktsv.cn/Article/details/gdayaukor.sHtML

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://www.share.fktsv.cn/Article/details/gqwxgrzxx.sHtML

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://m.share.sjlbkw.cn/Article/details/gahjbrbyb.sHtML

[N10] 链表节点定义
来源：http://mobile.epnwcf.com/Article/details/gccanohbb.sHtML

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://blog.tarul.cn/Article/details/gmamtejnj.sHtML

PHP:  class Node { public $v; public $next = null; }
来源：http://baike.epnwcf.com/Article/details/gsaccaqrc.sHtML

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://3g.vehdjk.com/Article/details/gaaasybzt.sHtML

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://blog.fktsv.cn/Article/details/gmggeqphf.sHtML

Java: class Node { int v; Node next; }
来源：http://3g.bbcook.cn/Article/details/gbyrgotpz.sHtML

Go:   type Node struct { V int; Next *Node }
来源：http://blog.sjlbkw.cn/Article/details/gvgqragzs.sHtML

Ruby: Node = Struct.new(:v, :next)
来源：http://www.share.vehdjk.com/Article/details/gjfepiavs.sHtML

C#:   class Node { public int V; public Node? Next; }
来源：http://baike.bbcook.cn/Article/details/glalbvwsn.sHtML

[N11] 二叉树中序遍历
来源：http://blog.bbcook.cn/Article/details/glaeobelr.sHtML

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://mobile.tarul.cn/Article/details/gimorkhkb.sHtML

PHP:  // 手写递归函数
来源：http://baike.tarul.cn/Article/details/grhrkgjxf.sHtML

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://blog.epnwcf.com/Article/details/gsqbbykos.sHtML

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://www.blog.fktsv.cn/Article/details/gysjzwpzd.sHtML

Java: // 手写递归
来源：http://m.share.epnwcf.com/Article/details/gfgkbhjbn.sHtML

Go:   // 手写递归
来源：http://blog.tarul.cn/Article/details/gflnwqgam.sHtML

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://www.blog.fktsv.cn/Article/details/gipqarqri.sHtML

C#:   // 手写递归
来源：http://m.share.tarul.cn/Article/details/gkhsmcrhy.sHtML

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://read.share.yfazqb.com/Article/details/gimtjvioi.sHtML

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://wap.vehdjk.com/Article/details/gctbgblva.sHtML

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://www.m.share.sjlbkw.cn/Article/details/gxqawagyb.sHtML

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/glchbwphh.sHtML

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://wap.sjlbkw.cn/Article/details/gkpistpcg.sHtML

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.bbcook.cn/Article/details/gsnwvcywe.sHtML

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mobile.vehdjk.com/Article/details/gdjwctolu.sHtML

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://www.share.epnwcf.com/Article/details/gvpiknbmb.sHtML

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://baike.sjlbkw.cn/Article/details/gicsdgvtx.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/ggzqoujfk.sHtML

O. 并发与异步
来源：http://3g.sjlbkw.cn/Article/details/gfzyeemvc.sHtML

================================================================================
来源：http://mobile.epnwcf.com/Article/details/gsgtkaxrk.sHtML

[O01] 启动一个线程
来源：http://wap.tarul.cn/Article/details/gghxjznnx.sHtML

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://mobile.fktsv.cn/Article/details/guowswyzv.sHtML

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://www.blog.yfazqb.com/Article/details/gdzcqlxqf.sHtML

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://wap.tarul.cn/Article/details/gqschshrb.sHtML

TS:   // 同 JS
来源：http://www.blog.vehdjk.com/Article/details/gwznfbwuc.sHtML

Java: new Thread(() -> f()).start()
来源：http://read.share.bbcook.cn/Article/details/grpxswfvl.sHtML

Go:   go f()
来源：http://3g.bbcook.cn/Article/details/gdluexubf.sHtML

Ruby: Thread.new { f }
来源：http://baike.bbcook.cn/Article/details/geqgmxdno.sHtML

C#:   Task.Run(() => F());
来源：http://baike.fktsv.cn/Article/details/gxnbjhlhr.sHtML

[O02] 使用线程池
来源：http://read.share.yfazqb.com/Article/details/gzanqqlhi.sHtML

Py:   concurrent.futures.ThreadPoolExecutor(max_workers=4)
来源：http://mobile.fktsv.cn/Article/details/gfmqytgum.sHtML

PHP:  // 用 Swoole / ReactPHP 等扩展实现
来源：http://m.share.tarul.cn/Article/details/govitedbp.sHtML

JS:   // worker_threads 线程池
来源：http://m.share.fktsv.cn/Article/details/gjuwcwafc.sHtML

TS:   // worker_threads 线程池
来源：http://www.m.share.bbcook.cn/Article/details/glybamaez.sHtML

Java: Executors.newFixedThreadPool(4)
来源：http://3g.bbcook.cn/Article/details/gvgzvehsk.sHtML

Go:   // 协程轻量，无需池；限并发用带缓冲 channel 当信号量
来源：http://www.share.sjlbkw.cn/Article/details/gixddvxcc.sHtML

Ruby: // 用 concurrent-ruby 的 ThreadPool
来源：http://blog.epnwcf.com/Article/details/gtwhieloa.sHtML

C#:   Task.WhenAll(...)  或 Parallel.ForEach
来源：http://wap.tarul.cn/Article/details/gwuvihlri.sHtML

[O03] 加锁保护共享数据
来源：http://baike.vehdjk.com/Article/details/gqerzkvve.sHtML

Py:   with lock: shared += 1
来源：http://www.m.share.sjlbkw.cn/Article/details/gcucnbxzs.sHtML

PHP:  // 用 flock() 做文件锁
来源：http://www.m.share.bbcook.cn/Article/details/gmvakvkyk.sHtML

JS:   // 单线程无需锁；跨线程共享内存用 Atomics
来源：http://www.m.share.yfazqb.com/Article/details/gyqbhnehf.sHtML

TS:   // 同 JS
来源：http://wap.epnwcf.com/Article/details/gqqgcpswt.sHtML

Java: synchronized (this) { shared++; }
来源：http://blog.bbcook.cn/Article/details/gfhbgrhrw.sHtML

Go:   mu.Lock();  defer mu.Unlock()
来源：http://baike.sjlbkw.cn/Article/details/gldwxfevw.sHtML

Ruby: mutex.synchronize { shared += 1 }
来源：http://www.m.share.sjlbkw.cn/Article/details/gvyiplbjp.sHtML

C#:   lock (gate) { shared++; }
来源：http://m.share.vehdjk.com/Article/details/gbygtbfez.sHtML

[O04] 定义异步函数并等待
来源：http://baike.fktsv.cn/Article/details/gbbmpppjq.sHtML

Py:   async def f():⏎    await g()
来源：http://m.share.yfazqb.com/Article/details/glffyslxl.sHtML

PHP:  // 无原生 async：用 Fiber 或 Swoole
来源：http://wap.fktsv.cn/Article/details/gdvohpaul.sHtML

JS:   async function f() { await g(); }
来源：http://wap.bbcook.cn/Article/details/gabnruepm.sHtML

TS:   async function f(): Promise<void> { await g(); }
来源：http://wap.yfazqb.com/Article/details/gwrithkwe.sHtML

Java: // 用 CompletableFuture 或虚拟线程
来源：http://m.share.sjlbkw.cn/Article/details/gyooocrzu.sHtML

Go:   // 无 async 关键字：直接 go 调用，用 channel 收结果
来源：http://baike.fktsv.cn/Article/details/gqidukxev.sHtML

Ruby: # 用 Fiber 或 async gem
来源：http://3g.sjlbkw.cn/Article/details/gxvxqvgli.sHtML

C#:   async Task F() { await G(); }
来源：http://mobile.tarul.cn/Article/details/gkhytfnma.sHtML

[O05] 并发执行并等待全部完成
来源：http://baike.vehdjk.com/Article/details/givuaagud.sHtML

Py:   asyncio.gather(*tasks)
来源：http://mobile.fktsv.cn/Article/details/gmjjwuqtn.sHtML

PHP:  // curl_multi 或 Amp 的 Promise\all
来源：http://www.blog.yfazqb.com/Article/details/gpcrzupkm.sHtML

JS:   await Promise.all(tasks)
来源：http://wap.sjlbkw.cn/Article/details/guvuxyeyb.sHtML

TS:   await Promise.all(tasks)
来源：http://www.share.sjlbkw.cn/Article/details/gquafnwqr.sHtML

Java: CompletableFuture.allOf(f1, f2).join()
来源：http://www.blog.epnwcf.com/Article/details/gvcibdrko.sHtML

Go:   sync.WaitGroup 或 errgroup.Wait()
来源：http://baike.yfazqb.com/Article/details/gczcbonws.sHtML

Ruby: threads.map(&:join)
来源：http://read.share.bbcook.cn/Article/details/gpwsnboep.sHtML

C#:   await Task.WhenAll(t1, t2)
来源：http://www.share.vehdjk.com/Article/details/gamwxbpbw.sHtML

[O06] 使用进程池
来源：http://read.share.bbcook.cn/Article/details/gmnvcktap.sHtML

Py:   concurrent.futures.ProcessPoolExecutor()
来源：http://read.share.yfazqb.com/Article/details/gxpexvwsa.sHtML

PHP:  // pcntl_fork 或多进程队列
来源：http://mobile.bbcook.cn/Article/details/gxafzmwrn.sHtML

JS:   // child_process / cluster 模块
来源：http://wap.epnwcf.com/Article/details/gideqwrct.sHtML

TS:   // child_process / cluster 模块
来源：http://blog.bbcook.cn/Article/details/gpyuntwno.sHtML

Java: // ForkJoinPool 或 ProcessBuilder
来源：http://m.share.sjlbkw.cn/Article/details/getqtyuki.sHtML

Go:   // goroutine 已占用多核，直接并发即可
来源：http://baike.sjlbkw.cn/Article/details/gekavxaiw.sHtML

Ruby: // fork 块
来源：http://mobile.vehdjk.com/Article/details/gcwseznlm.sHtML

C#:   Parallel.For
来源：http://blog.tarul.cn/Article/details/ggwveyqiz.sHtML

================================================================================
来源：http://3g.sjlbkw.cn/Article/details/glkhyvzop.sHtML

P. 常用工具函数
来源：http://wap.tarul.cn/Article/details/gytuqltke.sHtML

================================================================================
来源：http://3g.epnwcf.com/Article/details/gzjbzaawr.sHtML

[P01] 生成 UUID
来源：http://m.share.bbcook.cn/Article/details/geeuxgdot.sHtML

Py:   str(uuid.uuid4())
来源：http://blog.sjlbkw.cn/Article/details/gxfyegjfc.sHtML

PHP:  bin2hex(random_bytes(16));        // 或 ramsey/uuid
来源：http://3g.fktsv.cn/Article/details/gjyqphnbo.sHtML

JS:   crypto.randomUUID()
来源：http://wap.tarul.cn/Article/details/gjfldytru.sHtML

TS:   crypto.randomUUID()
来源：http://www.share.yfazqb.com/Article/details/gbwouixml.sHtML

Java: UUID.randomUUID().toString()
来源：http://www.blog.fktsv.cn/Article/details/glhhtyesi.sHtML

Go:   // 用 github.com/google/uuid
来源：http://www.blog.tarul.cn/Article/details/gxxslhfai.sHtML

Ruby: SecureRandom.uuid
来源：http://www.share.fktsv.cn/Article/details/gawnnxsxf.sHtML

C#:   Guid.NewGuid().ToString()
来源：http://read.share.sjlbkw.cn/Article/details/gpivythxj.sHtML

[P02] MD5 / SHA256 摘要
来源：http://read.share.yfazqb.com/Article/details/gqwwiysmr.sHtML

Py:   hashlib.sha256(b).hexdigest();  hashlib.md5(b).hexdigest()
来源：http://www.m.share.bbcook.cn/Article/details/gldjpvvgn.sHtML

PHP:  hash("sha256", $s);  md5($s);
来源：http://read.share.epnwcf.com/Article/details/gedqecxfx.sHtML

JS:   crypto.createHash("sha256").update(s).digest("hex")     // Node
来源：http://blog.yfazqb.com/Article/details/gnirquwxr.sHtML

TS:   crypto.createHash("sha256").update(s).digest("hex")
来源：http://www.m.share.fktsv.cn/Article/details/gdcmxacvf.sHtML

Java: MessageDigest.getInstance("SHA-256").digest(bytes)
来源：http://mobile.vehdjk.com/Article/details/gulizarec.sHtML

Go:   fmt.Sprintf("%x", sha256.Sum256([]byte(s)))
来源：http://www.share.sjlbkw.cn/Article/details/gxqxbqtuu.sHtML

Ruby: Digest::SHA256.hexdigest(s)
来源：http://baike.fktsv.cn/Article/details/gpirftsex.sHtML

C#:   Convert.ToHexString(SHA256.HashData(bytes))
来源：http://baike.tarul.cn/Article/details/grngetvim.sHtML

[P03] 生成短随机字符串
来源：http://www.blog.vehdjk.com/Article/details/gmnakmiwr.sHtML

Py:   "".join(random.choices(string.ascii_letters + string.digits, k=16))
来源：http://www.m.share.yfazqb.com/Article/details/gpmitqlbt.sHtML

PHP:  substr(str_shuffle(str_repeat("abcdefghijklmnopqrstuvwxyz0123456789", 2)), 0, 16);
来源：http://read.share.sjlbkw.cn/Article/details/gxlfjbpye.sHtML

JS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://baike.vehdjk.com/Article/details/gcyujjpyh.sHtML

TS:   [...crypto.getRandomValues(new Uint8Array(16))].map(b => (b % 36).toString(36)).join("")
来源：http://blog.epnwcf.com/Article/details/gsvucvuth.sHtML

Java: new BigInteger(130, new SecureRandom()).toString(36).substring(0, 16)
来源：http://www.blog.bbcook.cn/Article/details/guyduxjwr.sHtML

Go:   // crypto/rand 生成随机字节后 base64 或 hex 编码
来源：http://read.share.sjlbkw.cn/Article/details/geoyhkxhe.sHtML

Ruby: SecureRandom.alphanumeric(16)
来源：http://www.blog.bbcook.cn/Article/details/glddbupsr.sHtML

C#:   RandomNumberGenerator.GetHexString(16)     // .NET 8+
来源：http://3g.tarul.cn/Article/details/gvqshrqxs.sHtML

[P04] 求长度
来源：http://www.share.vehdjk.com/Article/details/gcyryotcm.sHtML


<!-- 参考信息 -->