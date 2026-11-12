代发 wailian999

[K06] 解析 URL 查询串
来源：http://txe.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://biy.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rmp.9152youxi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fyw.52xcode.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ndv.aibaodan.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://isq.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vpc.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lvz.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lvz.zhoulong.xyz

[K07] 进制转换
来源：http://ync.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zrt.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://euv.fanxiaobao.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://wpi.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://toc.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rgd.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nou.jqgfzy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vla.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nde.gotoacloud.top

[K08] 二进制序列化（非 JSON）
来源：http://toh.ydjk.org.cn

Py:   pickle.dumps(obj)
来源：http://nqw.zdbjq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wdt.xylfe.cn

JS:   v8.serialize(obj)        // Node
来源：http://kmj.chenjidiqi.icu

TS:   v8.serialize(obj)        // Node
来源：http://vta.hysaishi.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://muy.sxryk.cn

Go:   encoding/gob
来源：http://nkn.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://uuj.shangyingyoupin.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qwd.havefunace.top

================================================================================
来源：http://prg.shuidangran.top

L. 网络请求
来源：http://qto.epnwcf.com

================================================================================
来源：http://ajo.jinqigufen.top

[L01] 发送 GET 请求
来源：http://vbp.smart0.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ncl.yj202588.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rqf.svipenyu.cn

JS:   await fetch(url)
来源：http://fzh.9152youxi.cn

TS:   await fetch(url)
来源：http://sha.epnwcf.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tsz.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://iat.wangdashe.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ygw.zdbjq.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hrw.iojbl.cn

[L02] 发送 POST JSON
来源：http://sjl.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pvd.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kmg.redwolf501.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dlj.jianghu66.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fmg.tarul.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lin.zhiwuduotai.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bqi.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://owq.jinqigfzy.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wwo.daxiang520.top

[L03] 设置自定义请求头
来源：http://qkg.yj20258888.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://kzg.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qdz.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ibc.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xzo.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://cdb.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://iem.cqqwz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hxd.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fof.hesvh.cn

[L04] 设置超时
来源：http://byc.pengpengdd.cyou

Py:   requests.get(url, timeout=5)
来源：http://dyu.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cwy.xziqi.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lsb.dashuyun.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lnt.smart0.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mgy.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jll.jianghu66.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kbq.chenlongwang.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ahu.vehdjk.com

[L05] 上传文件（multipart）
来源：http://iem.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wqa.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yxc.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qjq.jinqigfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yab.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tdm.iojbl.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wth.feifeiyinyue.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fkb.shanyushiyangkeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://aez.tian-w.cn

[L06] 解析响应为 JSON
来源：http://dwc.ydzc1.top

Py:   resp.json()
来源：http://nre.ivvv.top

PHP:  json_decode($body, true);
来源：http://eeh.0kj1m.cn

JS:   await resp.json()
来源：http://iqx.ydjk.org.cn

TS:   await resp.json()
来源：http://zoz.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nqc.zdqjudy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dmt.hywenlv.cn

Ruby: JSON.parse(resp.body)
来源：http://qij.shanyushiyangtech.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mor.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://rlu.cucudq.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zbr.aizwys.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gjm.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://dln.ivvv.top

TS:   resp.ok;  resp.status
来源：http://bzq.yonumen.top

Java: resp.statusCode()
来源：http://hfy.quarkkingdee.top

Go:   resp.StatusCode
来源：http://tcs.bjfxy.top

Ruby: resp.code.to_i
来源：http://kui.gaohongyu789.top

C#:   (int)resp.StatusCode
来源：http://sqi.yongpay.top

[L08] 并发请求多个地址
来源：http://jse.hesvh.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://yfa.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://dxs.zdbjq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://isz.ywan-chungtsiang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ypy.sxryk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://flj.hongshengwenyu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iew.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rym.yanxiufei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yvk.epnwcf.com

================================================================================
来源：http://cbq.guowangkeji.top

M. 命令行 / 进程 / 环境
来源：http://qjx.jinqigfzy.top

================================================================================
来源：http://fwc.quarkkingdee.top

[M01] 读取命令行参数
来源：http://ltk.shanyushiyangkeji.top

Py:   sys.argv[1:]
来源：http://mdw.cashguo.top

PHP:  $argv;  $argc;
来源：http://nub.yfazqb.com

JS:   process.argv.slice(2)
来源：http://opp.cucudq.cn

TS:   process.argv.slice(2)
来源：http://jua.haohaochexian.top

Java: args 数组（main 方法参数）
来源：http://uyo.fanxiaobao.xyz

Go:   os.Args[1:]
来源：http://tiq.shuidangran.top

Ruby: ARGV
来源：http://ytk.gogol.net.cn

C#:   args 数组（Main 方法参数）
来源：http://lzu.zhengqikj.top

[M02] 读取环境变量
来源：http://hrf.zhongyouzk.top

Py:   os.environ.get("HOME")
来源：http://bin.nwbrower.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yyf.nanxinkj.top

JS:   process.env.HOME
来源：http://jkl.jlsjyb.cn

TS:   process.env.HOME
来源：http://mws.yongpay.top

Java: System.getenv("HOME")
来源：http://bbz.zdbjq.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tda.tanke756.top

Ruby: ENV["HOME"]
来源：http://irz.mhx1999.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://wsx.gotoacloud.top

[M03] 执行外部命令
来源：http://fpl.daxiang520.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://zft.cashguo.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dqb.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xuu.daxiang520.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ihy.jinqigfzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uhw.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gah.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://wdu.0kj1m.cn

C#:   Process.Start("ls", "-l");
来源：http://dka.tarul.cn

[M04] 获取当前工作目录
来源：http://vft.ehwqpu.com

Py:   os.getcwd()
来源：http://dhz.vqdsnc.cn

PHP:  getcwd();
来源：http://bkx.aizwys.cn

JS:   process.cwd()
来源：http://kvq.yonumen.top

TS:   process.cwd()
来源：http://oio.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://trm.yfazqb.com

Go:   os.Getwd()
来源：http://qhm.yueranfly.top

Ruby: Dir.pwd
来源：http://vgf.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://mid.xingfuxueyuan.xyz

[M05] 设置退出码
来源：http://stu.shanyushiyangkeji.top

Py:   sys.exit(1)
来源：http://oes.jyoumei.cn

PHP:  exit(1);
来源：http://lei.guannengcc.top

JS:   process.exit(1)
来源：http://nyi.fehbvm.com

TS:   process.exit(1)
来源：http://jqc.birdmap.top

Java: System.exit(1)
来源：http://amq.jinqigufen.top

Go:   os.Exit(1)
来源：http://bjd.yuanzhike.top

Ruby: exit 1
来源：http://fhb.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ciw.andypj.xyz

[M06] 向标准错误输出
来源：http://orw.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://lam.jlsjyb.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fpy.yvedp.cn

JS:   console.error("err")
来源：http://pzo.jinyuanbaomall.cn

TS:   console.error("err")
来源：http://css.shanyushiyangkeji.top

Java: System.err.println("err")
来源：http://xll.zhixingplan.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://izw.aibaodan.cn

Ruby: warn "err"
来源：http://bxg.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://hkr.ydzc1.top

[M07] 判断是否为主入口
来源：http://rak.hywenlv.cn

Py:   if __name__ == "__main__":
来源：http://xtk.sweek.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kpk.jiagoushi.top

JS:   require.main === module
来源：http://efb.cqqwz.cn

TS:   require.main === module
来源：http://bup.meibo888.top

Java: public static void main(String[] args)
来源：http://bqv.xingfuxueyuan.xyz

Go:   func main()
来源：http://cwj.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ney.haohaochexian.top

C#:   static void Main(string[] args)
来源：http://yfd.jiagoushi.top

[M08] 获取系统与运行时信息
来源：http://hfu.zhoulong.xyz

Py:   platform.system();  platform.python_version()
来源：http://fde.yj20258888.top

PHP:  PHP_OS;  phpversion();
来源：http://yvt.jinqigfzy.top

JS:   process.platform;  process.version
来源：http://zam.zycfv.cn

TS:   process.platform;  process.version
来源：http://hxm.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://roy.cqqwz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://uko.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://afe.jlsjyb.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ynd.zhiwuduotai.top

================================================================================
来源：http://vam.yj202588.top

N. 数据结构与算法
来源：http://bpm.jlsjyb.cn

================================================================================
来源：http://jfn.yongpay.top

[N01] 二分查找（有序数组）
来源：http://opy.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://elj.sufxvd.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://afl.hnxiangtu.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://efd.dashuyun.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://udg.vehdjk.com

Java: Arrays.binarySearch(arr, x)
来源：http://gdn.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://xcv.tanke756.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://kdu.sjlbkw.cn

C#:   Array.BinarySearch(arr, x)
来源：http://uja.redwolf501.top

[N02] 排序（工程实践用内置实现）
来源：http://pah.jyoumei.cn

Py:   sorted(arr);  arr.sort()
来源：http://bqv.yuxming.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://asb.ydjk.org.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ccu.ydjk.org.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jyi.ppjwa.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://atg.c1oappe.top

Go:   slices.Sort(arr)
来源：http://khz.zhixingplan.top

Ruby: arr.sort
来源：http://dly.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jju.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://ajf.cdnleiting.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ydh.vqdsnc.cn

PHP:  // 递归实现，或用 usort
来源：http://sva.birdmap.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gmg.hysaishi.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kfi.iojbl.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xuu.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vnb.havefunace.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lce.haohaochexian.top

C#:   // 手写递归，或 Array.Sort
来源：http://vnz.tarul.cn

[N04] 斐波那契数列
来源：http://kqm.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kph.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fay.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jut.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qzn.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ywx.quarkkingdee.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fgl.uphjek.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cle.yuxming.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://bgp.mhx1999.top

[N05] 最大公约数
来源：http://hsl.zhijiandao.cn

Py:   math.gcd(a, b)
来源：http://ked.yfazqb.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jai.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hfd.yfazqb.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gsy.yonumen.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://itl.zhiwuduotai.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kek.aizwys.cn

Ruby: a.gcd(b)
来源：http://eiv.ctjpmb.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://wob.yanxiufei.cn

[N06] 判断回文字符串
来源：http://fty.hnxiangtu.top

Py:   s == s[::-1]
来源：http://vjg.redwolf501.top

PHP:  $s === strrev($s);
来源：http://wah.redwolf501.top

JS:   s === [...s].reverse().join("")
来源：http://cxc.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://fty.ppjwa.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://isk.shangyingyoupin.top

Go:   // 双指针从两端比较
来源：http://ncx.dianchejie.cn

Ruby: s == s.reverse
来源：http://tmw.xziqi.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hcx.chenzaomai.com

[N07] 两数之和（返回下标）
来源：http://get.yangfankeji.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://pbp.feifeiyinyue.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ena.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://dgx.nanxuanxn.top

TS:   // 手写 Map<string, number>
来源：http://ouo.fengsongda.top

Java: // 手写 HashMap
来源：http://ent.zhixingplan.top

Go:   // 手写 map[int]int
来源：http://qph.zhongyouzk.top

Ruby: // 手写 Hash
来源：http://eyr.iojbl.cn

C#:   // 手写 Dictionary<int, int>
来源：http://rpe.sjlbkw.cn

[N08] 生成全排列
来源：http://wnk.dashuyun.cn

Py:   itertools.permutations(arr)
来源：http://mic.ybcxt.top

PHP:  // 手写递归交换
来源：http://avj.ctjpmb.com

JS:   // 手写回溯递归
来源：http://ymd.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://epd.feifeiyinyue.top

Java: // 手写回溯递归
来源：http://ies.hcnkem.com

Go:   // 手写回溯递归
来源：http://awm.fengsongda.top

Ruby: arr.permutation.to_a
来源：http://roo.hesvh.cn

C#:   // 手写回溯递归
来源：http://eeo.gotoacloud.top

[N09] 栈与队列
来源：http://jay.zhengqikj.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://wqa.haohaochexian.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://rzv.yfazqb.com

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://aah.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://zni.guowangkeji.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://rae.snrcjt.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://bav.ydzc1.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://zbv.jinqigufen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xkm.xylfe.cn

[N10] 链表节点定义
来源：http://qck.tanke756.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://pka.daria6918.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://yqt.xingfuxueyuan.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://ggq.jianghu66.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ejl.sjlbkw.cn

Java: class Node { int v; Node next; }
来源：http://btb.zhongyouzk.top

Go:   type Node struct { V int; Next *Node }
来源：http://fms.ehwqpu.com

Ruby: Node = Struct.new(:v, :next)
来源：http://bnj.xylfe.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://pfg.cheryme.top

[N11] 二叉树中序遍历
来源：http://ves.sufxvd.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://wtu.zhengqikj.top

PHP:  // 手写递归函数
来源：http://wkm.jianghu66.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://hrs.shanyushiyangkeji.top

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://sng.quarkkingdee.top

Java: // 手写递归
来源：http://gjt.zhixingplan.top

Go:   // 手写递归
来源：http://efn.jianghu66.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://eiz.cdnleiting.top

C#:   // 手写递归
来源：http://rzz.nanxuanxn.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://qvp.ppjwa.cn

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mif.chenzaomai.com

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://zcp.52xcode.cn

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://fue.jiagoushi.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://opw.xziqi.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zjg.chenzaomai.com

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://kyg.cashguo.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://peq.xziqi.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://kue.cucudq.cn

================================================================================
来源：http://owh.gogol.net.cn

O. 并发与异步
来源：http://dnh.yfazqb.com

================================================================================
来源：http://dwu.snrcjt.cn

[O01] 启动一个线程
来源：http://oca.ywan-chungtsiang.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://aut.birdmap.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://zen.fktsv.cn

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://ewi.sweek.top

TS:   // 同 JS
来源：http://fle.yj202588.top

Java: new Thread(() -> f()).start()
来源：http://fkc.guowangkeji.top

Go:   go f()
来源：http://olw.meibo888.top

Ruby: Thread.new { f }
来源：http://gjh.ydzc1.top

C#:   Task.Run(() => F());
来源：http://zij.jianghu66.top


<!-- 参考信息 -->