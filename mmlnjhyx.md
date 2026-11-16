代发 wailian999

Py:   copy.deepcopy(obj)
来源：http://rce.xziqi.cn

PHP:  unserialize(serialize($obj));
来源：http://khm.hcnkem.com

JS:   structuredClone(obj)
来源：http://djb.gogol.net.cn

TS:   structuredClone(obj)
来源：http://jmc.sxryk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://oal.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qwd.zdbjq.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xay.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mkc.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://ryi.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xfz.yuanzhike.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kge.fehbvm.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ufa.yonumen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://wpl.shuidangran.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pjp.gaohongyu789.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tzo.birdmap.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cil.hysaishi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://cfy.mhx1999.top

[K07] 进制转换
来源：http://beb.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wez.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://cbr.tianlin.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fzv.fanxiaobao.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nsg.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hmp.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zka.zhijiandao.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cph.zhaomingkeji.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cpt.nwbrower.top

[K08] 二进制序列化（非 JSON）
来源：http://syw.cqqwz.cn

Py:   pickle.dumps(obj)
来源：http://ayq.jinyuanbaomall.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ujj.aibaodan.cn

JS:   v8.serialize(obj)        // Node
来源：http://wde.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://gdo.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xiy.fehbvm.com

Go:   encoding/gob
来源：http://hlr.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://iws.xuanzx.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zdp.zhaomingkeji.xyz

================================================================================
来源：http://lzw.jqgufenzy.top

L. 网络请求
来源：http://zav.jinqigfzy.top

================================================================================
来源：http://tjd.bbcook.cn

[L01] 发送 GET 请求
来源：http://lnl.zhijiandao.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oxe.chenlongwang.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://inu.0kj1m.cn

JS:   await fetch(url)
来源：http://hzl.sxryk.cn

TS:   await fetch(url)
来源：http://dgv.aibaodan.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tjz.daxiang520.top

Go:   resp, err := http.Get(url)
来源：http://xxl.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://koq.xingfuxueyuan.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ymb.yj202588.top

[L02] 发送 POST JSON
来源：http://lbe.wangshuangyany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ztx.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hwo.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hmg.dianchejie.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ttx.vehdjk.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://iac.pycfn.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ucz.pengpengdd.cyou

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uux.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qgl.yangfankeji.com

[L03] 设置自定义请求头
来源：http://rkm.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://skm.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://brx.kuanghao11.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zbs.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dij.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://eaj.shanyushiyangtech.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fci.meibo888.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qiv.0kj1m.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://usc.xuanzx.com

[L04] 设置超时
来源：http://wqf.hywenlv.cn

Py:   requests.get(url, timeout=5)
来源：http://rcs.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uda.haohaochexian.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wxz.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xho.cqqwz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://knj.zycfv.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aeu.jlsjyb.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jzp.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ref.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://qfl.yueranfly.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fbh.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://scq.yj20258888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lln.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://uex.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xrz.uphjek.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jtc.epnwcf.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://cop.shangyingyoupin.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yod.tarul.cn

[L06] 解析响应为 JSON
来源：http://pfx.mhx1999.top

Py:   resp.json()
来源：http://len.zhixingplan.top

PHP:  json_decode($body, true);
来源：http://rpr.wangshuangyany.cn

JS:   await resp.json()
来源：http://pmy.ydzc1.top

TS:   await resp.json()
来源：http://usg.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rni.sweek.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://thj.zhongyouzk.top

Ruby: JSON.parse(resp.body)
来源：http://obp.yueranfly.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://tvg.zycfv.cn

[L07] 处理 HTTP 状态码
来源：http://pge.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ahz.guannengcc.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://etj.yonumen.top

JS:   resp.ok;  resp.status
来源：http://gsm.guannengcc.top

TS:   resp.ok;  resp.status
来源：http://ull.yj202588.top

Java: resp.statusCode()
来源：http://lnb.yanxiufei.cn

Go:   resp.StatusCode
来源：http://xvz.sysykeji.top

Ruby: resp.code.to_i
来源：http://ifn.jlsjyb.cn

C#:   (int)resp.StatusCode
来源：http://abv.hysaishi.cn

[L08] 并发请求多个地址
来源：http://yqo.zdqjudy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zfm.hcnkem.com

PHP:  curl_multi_init() 系列
来源：http://yus.tian-w.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kyn.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pxg.chenjidiqi.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vzp.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://bge.kuanghao11.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://gme.haohaochexian.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lfm.hnxiangtu.top

================================================================================
来源：http://ugu.yuxming.cn

M. 命令行 / 进程 / 环境
来源：http://fdp.birdmap.top

================================================================================
来源：http://uys.guowangkeji.top

[M01] 读取命令行参数
来源：http://tab.yangfankeji.com

Py:   sys.argv[1:]
来源：http://wif.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://qhs.jinqigufen.top

JS:   process.argv.slice(2)
来源：http://dyr.zdbjq.cn

TS:   process.argv.slice(2)
来源：http://yju.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://pje.mhx1999.top

Go:   os.Args[1:]
来源：http://znt.fengsongda.top

Ruby: ARGV
来源：http://rte.jinghuilouyu.cn

C#:   args 数组（Main 方法参数）
来源：http://rwb.hnxiangtu.top

[M02] 读取环境变量
来源：http://rrp.chenzaomai.com

Py:   os.environ.get("HOME")
来源：http://ycb.xylfe.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jfn.svipenyu.cn

JS:   process.env.HOME
来源：http://ivd.hnqzz.top

TS:   process.env.HOME
来源：http://odu.chenlongwang.top

Java: System.getenv("HOME")
来源：http://sxy.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ntm.pycfn.com

Ruby: ENV["HOME"]
来源：http://ppt.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://iai.hcnkem.com

[M03] 执行外部命令
来源：http://hyc.tarul.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cye.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lpo.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xub.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://oht.jinqigufen.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://syl.tianlin.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://fsb.jinyuanbaomall.cn

Ruby: system("ls -l");  `ls -l`
来源：http://frz.vqdsnc.cn

C#:   Process.Start("ls", "-l");
来源：http://jic.haohaochexian.top

[M04] 获取当前工作目录
来源：http://tga.shuidangran.top

Py:   os.getcwd()
来源：http://iun.jiagoushi.top

PHP:  getcwd();
来源：http://tzd.havefunace.top

JS:   process.cwd()
来源：http://vvy.xziqi.cn

TS:   process.cwd()
来源：http://lfw.316326.xyz

Java: Path.of("").toAbsolutePath()
来源：http://uve.hfpthk.cn

Go:   os.Getwd()
来源：http://lsk.hcnkem.com

Ruby: Dir.pwd
来源：http://nka.ywan-chungtsiang.top

C#:   Directory.GetCurrentDirectory()
来源：http://ika.yongpay.top

[M05] 设置退出码
来源：http://gat.hnxiangtu.top

Py:   sys.exit(1)
来源：http://kvv.bbcook.cn

PHP:  exit(1);
来源：http://jqi.snrcjt.cn

JS:   process.exit(1)
来源：http://ggt.meibo888.top

TS:   process.exit(1)
来源：http://end.dashuyun.cn

Java: System.exit(1)
来源：http://ufp.zdbjq.cn

Go:   os.Exit(1)
来源：http://xzr.vqdsnc.cn

Ruby: exit 1
来源：http://uix.ivvv.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://urs.ywan-chungtsiang.top

[M06] 向标准错误输出
来源：http://gnh.zhixingplan.top

Py:   print("err", file=sys.stderr)
来源：http://awj.shanyushiyangkeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bsc.ydzc1.top

JS:   console.error("err")
来源：http://yvu.shanyushiyangtech.top

TS:   console.error("err")
来源：http://uti.sweek.top

Java: System.err.println("err")
来源：http://qoe.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tgo.sjlbkw.cn

Ruby: warn "err"
来源：http://aiq.ydzc1.top

C#:   Console.Error.WriteLine("err")
来源：http://tga.xylfe.cn

[M07] 判断是否为主入口
来源：http://cpu.zdbjq.cn

Py:   if __name__ == "__main__":
来源：http://xdm.yvedp.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hdl.daxiang520.top

JS:   require.main === module
来源：http://ymu.gogol.net.cn

TS:   require.main === module
来源：http://ycc.zycfv.cn

Java: public static void main(String[] args)
来源：http://phf.xuanzx.com

Go:   func main()
来源：http://ehu.jiagoushi.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gok.birdmap.top

C#:   static void Main(string[] args)
来源：http://ieq.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://sdo.pengpengdd.cyou

Py:   platform.system();  platform.python_version()
来源：http://ztw.gzhubu.top

PHP:  PHP_OS;  phpversion();
来源：http://urp.wangdashe.top

JS:   process.platform;  process.version
来源：http://gmg.cucudq.cn

TS:   process.platform;  process.version
来源：http://icr.sufxvd.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xww.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tjb.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rvl.meibo888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gvn.fzhhl.top

================================================================================
来源：http://dky.smart0.xyz

N. 数据结构与算法
来源：http://lax.andypj.xyz

================================================================================
来源：http://aqp.zhixingplan.top

[N01] 二分查找（有序数组）
来源：http://mqk.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://iic.ctjpmb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wte.yangfankeji.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rwp.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rcn.jqgufenzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://qhm.dashuyun.cn

Go:   sort.SearchInts(arr, x)
来源：http://jme.zhengqikj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hnt.nanxinkj.top

C#:   Array.BinarySearch(arr, x)
来源：http://scf.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://bdy.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://zuo.wangshuangyany.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mdi.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cam.yuanzhike.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://htf.yj20258888.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lou.yj20258888.top

Go:   slices.Sort(arr)
来源：http://phr.jyoumei.cn

Ruby: arr.sort
来源：http://don.hywenlv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lfo.gogol.net.cn

[N03] 快速排序（分治示例）
来源：http://hwo.chenzaomai.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jwz.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://fvu.sjlbkw.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tsg.yongpay.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xyr.hongshengwenyu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://pcm.jyoumei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bzp.yuxming.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zuo.uphjek.com

C#:   // 手写递归，或 Array.Sort
来源：http://hxg.feifeiyinyue.top

[N04] 斐波那契数列
来源：http://xbj.gotoacloud.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://bjz.jqgufenzy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kji.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sxu.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hyq.bjfxy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tjp.feifeiyinyue.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lpj.xuetiantiany.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vew.ywan-chungtsiang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hnd.nanxuanxn.top

[N05] 最大公约数
来源：http://qez.0kj1m.cn

Py:   math.gcd(a, b)
来源：http://yse.feifeiyinyue.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cjz.zdbjq.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dbk.quarkkingdee.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://leg.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zbl.shangyingyoupin.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://acv.daria6918.cn

Ruby: a.gcd(b)
来源：http://apt.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sxp.zhiwuduotai.top

[N06] 判断回文字符串
来源：http://ijx.yangfankeji.com

Py:   s == s[::-1]
来源：http://lnv.fzhhl.top

PHP:  $s === strrev($s);
来源：http://kms.zhongyouzk.top

JS:   s === [...s].reverse().join("")
来源：http://zlq.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://poh.hysaishi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ruk.hnqzz.top

Go:   // 双指针从两端比较
来源：http://bsb.hywenlv.cn

Ruby: s == s.reverse
来源：http://fwb.chenzaomai.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://jxi.svipenyu.cn

[N07] 两数之和（返回下标）
来源：http://gql.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ubd.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aqw.xuanzx.com

JS:   // 手写 Map：map.set(v, i)
来源：http://tgk.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://lqu.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://lne.jinghuilouyu.cn

Go:   // 手写 map[int]int
来源：http://epi.gogol.net.cn

Ruby: // 手写 Hash
来源：http://wgf.shangyingyoupin.top

C#:   // 手写 Dictionary<int, int>
来源：http://ddy.c1oappe.top

[N08] 生成全排列
来源：http://ufp.zdbjq.cn

Py:   itertools.permutations(arr)
来源：http://hje.ctjpmb.com

PHP:  // 手写递归交换
来源：http://doj.hcnkem.com

JS:   // 手写回溯递归
来源：http://puv.zhixingplan.top

TS:   // 手写回溯递归
来源：http://hib.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://bqb.nwbrower.top

Go:   // 手写回溯递归
来源：http://sux.xuetiantiany.cn

Ruby: arr.permutation.to_a
来源：http://bhn.vehdjk.com

C#:   // 手写回溯递归
来源：http://rwv.cdnleiting.top

[N09] 栈与队列
来源：http://fnp.jinqigufen.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://cfk.kuanghao11.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://hid.shangyingyoupin.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://jkr.zdqjudy.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://anv.jyoumei.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://stk.yuanzhike.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://moo.xuetiantiany.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://apg.316326.xyz

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jbg.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://kyb.ybcxt.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://xsm.ivvv.top

PHP:  class Node { public $v; public $next = null; }
来源：http://itb.ppjwa.cn

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://jxn.gogol.net.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://rdu.chenzaomai.com

Java: class Node { int v; Node next; }
来源：http://wce.jiagoushi.top

Go:   type Node struct { V int; Next *Node }
来源：http://jpq.epnwcf.com

Ruby: Node = Struct.new(:v, :next)
来源：http://okl.havefunace.top

C#:   class Node { public int V; public Node? Next; }
来源：http://dvr.fktsv.cn

[N11] 二叉树中序遍历
来源：http://piw.gogol.net.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://nuh.hnxiangtu.top

PHP:  // 手写递归函数
来源：http://ejz.cdnleiting.top

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://gqd.tianlin.xyz

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://ztw.jinghuilouyu.cn

Java: // 手写递归
来源：http://tmi.sjlbkw.cn

Go:   // 手写递归
来源：http://pny.fehbvm.com

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://hsh.cdnleiting.top

C#:   // 手写递归
来源：http://ydk.mhx1999.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mkd.ivvv.top

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://vju.tarul.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://jdm.smart0.xyz

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://sqo.yj20258.top

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://pba.jiagoushi.top

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://zfv.redwolf501.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://gen.jqgufenzy.top

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://saj.cqqwz.cn

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://hsw.vqdsnc.cn

================================================================================
来源：http://lkx.ywan-chungtsiang.top

O. 并发与异步
来源：http://kue.yongpay.top

================================================================================
来源：http://lae.zhijiandao.cn

[O01] 启动一个线程
来源：http://myt.cdnleiting.top


<!-- 参考信息 -->