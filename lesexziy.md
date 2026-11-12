代发 wailian999

[K06] 解析 URL 查询串
来源：http://esw.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fsz.iojbl.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mwb.jqgfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jix.ivvv.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gpl.hcnkem.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://llt.zdqjudy.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://boq.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ctb.redwolf501.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pew.nwbrower.top

[K07] 进制转换
来源：http://lwh.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zgb.guowangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zoz.xuanzx.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qen.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pdp.xuanzx.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://eiv.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://qmw.zdqjudy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://suj.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ogl.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://wwj.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://uzw.havefunace.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bti.daxiang520.top

JS:   v8.serialize(obj)        // Node
来源：http://anr.hnqzz.top

TS:   v8.serialize(obj)        // Node
来源：http://obx.sxryk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rtq.yongpay.top

Go:   encoding/gob
来源：http://fne.aizwys.cn

Ruby: Marshal.dump(obj)
来源：http://wlw.hnxiangtu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://uty.vehdjk.com

================================================================================
来源：http://xaq.tianlin.xyz

L. 网络请求
来源：http://lid.cheryme.top

================================================================================
来源：http://flf.yfazqb.com

[L01] 发送 GET 请求
来源：http://cro.sjlbkw.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tqi.yj202588.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://gwp.gzhubu.top

JS:   await fetch(url)
来源：http://ukw.chenjidiqi.icu

TS:   await fetch(url)
来源：http://lto.tian-w.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gcr.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://iwb.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bca.jiagoushi.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://quu.gotoacloud.top

[L02] 发送 POST JSON
来源：http://diy.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://xux.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ogb.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://sbj.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zec.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dvu.ybcxt.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lac.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://izr.fehbvm.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qjt.fehbvm.com

[L03] 设置自定义请求头
来源：http://fvm.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gau.yuxming.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dyz.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ayv.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://inm.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://msr.aizwys.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jau.jlsjyb.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vvx.yvedp.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kvz.xziqi.cn

[L04] 设置超时
来源：http://rpa.aibaodan.cn

Py:   requests.get(url, timeout=5)
来源：http://irj.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://sva.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jlr.vqdsnc.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vxm.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zfr.gaohongyu789.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sqb.vehdjk.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ubx.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nyd.tarul.cn

[L05] 上传文件（multipart）
来源：http://dsw.fanxiaobao.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jfs.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://orv.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://bso.yj20258888.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mjh.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://atv.wangshuangyany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qtp.sysykeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://egv.316326.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://uiv.c1oappe.top

[L06] 解析响应为 JSON
来源：http://zko.nwbrower.top

Py:   resp.json()
来源：http://kow.xuanzx.com

PHP:  json_decode($body, true);
来源：http://ngt.svipenyu.cn

JS:   await resp.json()
来源：http://mjc.jinyuanbaomall.cn

TS:   await resp.json()
来源：http://tmc.shzxlz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tdq.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kuk.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://qzo.gzhubu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://eqi.yanxiufei.cn

[L07] 处理 HTTP 状态码
来源：http://oye.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sbg.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://egp.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://sqd.cheryme.top

TS:   resp.ok;  resp.status
来源：http://cqw.ybcxt.top

Java: resp.statusCode()
来源：http://hnm.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://yic.tianlin.xyz

Ruby: resp.code.to_i
来源：http://lzv.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://kgm.shzxlz.cn

[L08] 并发请求多个地址
来源：http://ytt.zycfv.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kdz.yueranfly.top

PHP:  curl_multi_init() 系列
来源：http://kvz.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ulw.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vdy.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vto.shanyushiyangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pgm.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qpf.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sfk.hcnkem.com

================================================================================
来源：http://lbe.sufxvd.cn

M. 命令行 / 进程 / 环境
来源：http://bpi.yj202588.top

================================================================================
来源：http://evy.yj202588.top

[M01] 读取命令行参数
来源：http://hzl.xinyue.icu

Py:   sys.argv[1:]
来源：http://zpk.aizwys.cn

PHP:  $argv;  $argc;
来源：http://ust.hammf.cn

JS:   process.argv.slice(2)
来源：http://las.jiagoushi.top

TS:   process.argv.slice(2)
来源：http://ozx.sufxvd.cn

Java: args 数组（main 方法参数）
来源：http://apj.cqqwz.cn

Go:   os.Args[1:]
来源：http://lex.xinyue.icu

Ruby: ARGV
来源：http://dfx.cheryme.top

C#:   args 数组（Main 方法参数）
来源：http://lhh.yvedp.cn

[M02] 读取环境变量
来源：http://bvj.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://mxw.nanxuanxn.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iqe.yj20258.top

JS:   process.env.HOME
来源：http://fgs.hysaishi.cn

TS:   process.env.HOME
来源：http://hnx.shzxlz.cn

Java: System.getenv("HOME")
来源：http://mxp.yvedp.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gdl.52xcode.cn

Ruby: ENV["HOME"]
来源：http://omd.cheryme.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qlu.jianghu66.top

[M03] 执行外部命令
来源：http://wmj.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rdv.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://omz.yj20258.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mgk.jinghuilouyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://mpy.shanyushiyangtech.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ttt.chenzaomai.com

Go:   exec.Command("ls", "-l").Output()
来源：http://nhj.yj202588.top

Ruby: system("ls -l");  `ls -l`
来源：http://ynu.zhengqikj.top

C#:   Process.Start("ls", "-l");
来源：http://und.yonumen.top

[M04] 获取当前工作目录
来源：http://jno.yangfankeji.com

Py:   os.getcwd()
来源：http://oth.sxryk.cn

PHP:  getcwd();
来源：http://eua.zdbjq.cn

JS:   process.cwd()
来源：http://ibq.zdqjudy.top

TS:   process.cwd()
来源：http://coz.bjfxy.top

Java: Path.of("").toAbsolutePath()
来源：http://oao.gzhubu.top

Go:   os.Getwd()
来源：http://syr.wangdashe.top

Ruby: Dir.pwd
来源：http://blb.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://abg.uphjek.com

[M05] 设置退出码
来源：http://pqr.gotoacloud.top

Py:   sys.exit(1)
来源：http://qyn.shangyingyoupin.top

PHP:  exit(1);
来源：http://bdw.hnxiangtu.top

JS:   process.exit(1)
来源：http://nfm.redwolf501.top

TS:   process.exit(1)
来源：http://brz.jiagoushi.top

Java: System.exit(1)
来源：http://noo.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://fqx.jinqigufen.top

Ruby: exit 1
来源：http://tuo.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tee.hfpthk.cn

[M06] 向标准错误输出
来源：http://qyt.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://fjo.daria6918.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://qfe.yj20258888.top

JS:   console.error("err")
来源：http://aim.9152youxi.cn

TS:   console.error("err")
来源：http://nrr.hnxiangtu.top

Java: System.err.println("err")
来源：http://euw.9152youxi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xln.cqqwz.cn

Ruby: warn "err"
来源：http://pvb.cdnleiting.top

C#:   Console.Error.WriteLine("err")
来源：http://cjq.zycfv.cn

[M07] 判断是否为主入口
来源：http://oql.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://gjw.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://cmd.fanxiaobao.xyz

JS:   require.main === module
来源：http://zrv.xuanzx.com

TS:   require.main === module
来源：http://rhr.snrcjt.cn

Java: public static void main(String[] args)
来源：http://qqw.sufxvd.cn

Go:   func main()
来源：http://mge.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rto.52xcode.cn

C#:   static void Main(string[] args)
来源：http://iuc.zhijiandao.cn

[M08] 获取系统与运行时信息
来源：http://lbh.jqgfzy.top

Py:   platform.system();  platform.python_version()
来源：http://xcf.svipenyu.cn

PHP:  PHP_OS;  phpversion();
来源：http://piq.yfazqb.com

JS:   process.platform;  process.version
来源：http://gve.havefunace.top

TS:   process.platform;  process.version
来源：http://hud.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tkr.wangshuangyany.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://srh.zhiwuduotai.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eyg.ehwqpu.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://tup.shzxlz.cn

================================================================================
来源：http://psp.bbcook.cn

N. 数据结构与算法
来源：http://xnm.hongshengwenyu.top

================================================================================
来源：http://gmp.fktsv.cn

[N01] 二分查找（有序数组）
来源：http://moc.hfpthk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ikn.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qzj.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hqk.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kib.wangdashe.top

Java: Arrays.binarySearch(arr, x)
来源：http://tcq.hcnkem.com

Go:   sort.SearchInts(arr, x)
来源：http://vuk.ppjwa.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dqx.tanke756.top

C#:   Array.BinarySearch(arr, x)
来源：http://ijg.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://iag.epnwcf.com

Py:   sorted(arr);  arr.sort()
来源：http://owy.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://olw.zdbjq.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://jfy.dianchejie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://voq.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vta.c1oappe.top

Go:   slices.Sort(arr)
来源：http://lck.jlsjyb.cn

Ruby: arr.sort
来源：http://uad.yonumen.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ohw.zhongyouzk.top

[N03] 快速排序（分治示例）
来源：http://vcj.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ozy.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://kzt.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hpc.nanxinkj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xnu.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pcg.gotoacloud.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qip.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://whl.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://cte.xziqi.cn

[N04] 斐波那契数列
来源：http://rip.cqqwz.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qfm.shanyushiyangtech.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kjx.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rdx.hnxiangtu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qym.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tma.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://uon.ybcxt.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kei.sjlbkw.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qwa.zhaomingkeji.xyz

[N05] 最大公约数
来源：http://fzq.yonumen.top

Py:   math.gcd(a, b)
来源：http://kzq.nwbrower.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mfe.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rae.feifeiyinyue.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://szg.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fvj.chenjidiqi.icu

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bkb.hnxiangtu.top

Ruby: a.gcd(b)
来源：http://uuz.ywan-chungtsiang.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oam.zhaomingkeji.xyz

[N06] 判断回文字符串
来源：http://ysg.chenzaomai.com

Py:   s == s[::-1]
来源：http://kxy.9152youxi.cn

PHP:  $s === strrev($s);
来源：http://kxu.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://nmd.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://ccj.jqgufenzy.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oft.ctjpmb.com

Go:   // 双指针从两端比较
来源：http://vnd.dashuyun.cn

Ruby: s == s.reverse
来源：http://rnd.aibaodan.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ifr.sysykeji.top

[N07] 两数之和（返回下标）
来源：http://sbx.yuanzhike.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wup.vqdsnc.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zst.bbcook.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cga.cucudq.cn

TS:   // 手写 Map<string, number>
来源：http://dem.yj202588.top

Java: // 手写 HashMap
来源：http://ewq.nanxinkj.top

Go:   // 手写 map[int]int
来源：http://wlj.aizwys.cn

Ruby: // 手写 Hash
来源：http://pbl.nanxuanxn.top

C#:   // 手写 Dictionary<int, int>
来源：http://xqn.zhixingplan.top

[N08] 生成全排列
来源：http://ilv.sysykeji.top

Py:   itertools.permutations(arr)
来源：http://rnw.ydzc1.top

PHP:  // 手写递归交换
来源：http://xnj.jlsjyb.cn

JS:   // 手写回溯递归
来源：http://jeq.smart0.xyz

TS:   // 手写回溯递归
来源：http://yql.tanke756.top

Java: // 手写回溯递归
来源：http://qlm.dianchejie.cn

Go:   // 手写回溯递归
来源：http://nlv.jyoumei.cn

Ruby: arr.permutation.to_a
来源：http://kgv.zhongyouzk.top

C#:   // 手写回溯递归
来源：http://kvq.sysykeji.top

[N09] 栈与队列
来源：http://mnw.guannengcc.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://daf.shanyushiyangtech.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://yfl.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://lqd.jqgufenzy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://aqk.ctjpmb.com

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sjo.zdqjudy.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://esb.yanxiufei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://mhw.snrcjt.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://dqx.gogol.net.cn

[N10] 链表节点定义
来源：http://zjl.yongpay.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://lkx.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://phr.yangfankeji.com

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ahu.andypj.xyz

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rzb.jqgfzy.top

Java: class Node { int v; Node next; }
来源：http://vnu.jinqigfzy.top

Go:   type Node struct { V int; Next *Node }
来源：http://omh.yj202588.top

Ruby: Node = Struct.new(:v, :next)
来源：http://qau.jinghuilouyu.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://fik.ivvv.top

[N11] 二叉树中序遍历
来源：http://qwy.snrcjt.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://ggw.meibo888.top

PHP:  // 手写递归函数
来源：http://xro.fehbvm.com

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ypg.yonumen.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://agt.9152youxi.cn

Java: // 手写递归
来源：http://gay.gogol.net.cn

Go:   // 手写递归
来源：http://zgf.uphjek.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://fvq.haohaochexian.top

C#:   // 手写递归
来源：http://oze.jinyuanbaomall.cn

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://rsx.tarul.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://ulg.fktsv.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://daq.haohaochexian.top

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nxl.sjlbkw.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://nmi.yueranfly.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zzi.yvedp.cn

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://mgy.tian-w.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://uon.yuanzhike.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://ltt.jinyuanbaomall.cn

================================================================================
来源：http://dac.pycfn.com

O. 并发与异步
来源：http://ufx.zhengqikj.top

================================================================================
来源：http://afu.c1oappe.top

[O01] 启动一个线程
来源：http://sam.guowangkeji.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://zjc.gogol.net.cn

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://sjd.ehwqpu.com

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://lzd.chenjidiqi.icu

TS:   // 同 JS
来源：http://ygt.sjlbkw.cn

Java: new Thread(() -> f()).start()
来源：http://ijy.xuanzx.com

Go:   go f()
来源：http://fji.jinyuanbaomall.cn

Ruby: Thread.new { f }
来源：http://ufu.jyoumei.cn

C#:   Task.Run(() => F());
来源：http://djz.yanxiufei.cn


<!-- 参考信息 -->