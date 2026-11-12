代发 wailian999

[K06] 解析 URL 查询串
来源：http://pzr.daxiang520.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://msn.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pbf.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fax.c1oappe.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vxc.xinyue.icu

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://yfv.tarul.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iig.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://coj.havefunace.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ntn.sjlbkw.cn

[K07] 进制转换
来源：http://obh.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ypu.jinqigfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://txc.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://odt.feifeiyinyue.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ppz.yj20258.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bmn.jinqigufen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://koa.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lcf.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://lms.yvedp.cn

[K08] 二进制序列化（非 JSON）
来源：http://dsk.yfazqb.com

Py:   pickle.dumps(obj)
来源：http://pyo.jiagoushi.top

PHP:  serialize($obj);  unserialize($s);
来源：http://phm.jyoumei.cn

JS:   v8.serialize(obj)        // Node
来源：http://hys.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://ewi.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://nss.hcnkem.com

Go:   encoding/gob
来源：http://ubf.jinqigufen.top

Ruby: Marshal.dump(obj)
来源：http://qyi.zdqjudy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fol.zhiwuduotai.top

================================================================================
来源：http://ebb.epnwcf.com

L. 网络请求
来源：http://tyw.ehwqpu.com

================================================================================
来源：http://ybo.fktsv.cn

[L01] 发送 GET 请求
来源：http://teg.tarul.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://bid.gzhubu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pzc.ehwqpu.com

JS:   await fetch(url)
来源：http://bvf.sysykeji.top

TS:   await fetch(url)
来源：http://kfm.jyoumei.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oaf.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://mts.vqdsnc.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://kgh.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nzl.bbcook.cn

[L02] 发送 POST JSON
来源：http://tph.9152youxi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://pdg.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pxd.aibaodan.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ahg.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jin.cashguo.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gjq.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zqw.shangyingyoupin.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://djg.chenjidiqi.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://drk.hcnkem.com

[L03] 设置自定义请求头
来源：http://nve.feifeiyinyue.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nsk.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aje.jqgfzy.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wtb.snrcjt.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gyh.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xxe.shanyushiyangkeji.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gbh.chenlongwang.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bkw.jiagoushi.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iog.fengsongda.top

[L04] 设置超时
来源：http://wfk.sysykeji.top

Py:   requests.get(url, timeout=5)
来源：http://rtp.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oku.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fof.nwbrower.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ihp.ehwqpu.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oia.ppjwa.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://oev.zhaomingkeji.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vlc.nwbrower.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jmu.sweek.top

[L05] 上传文件（multipart）
来源：http://pmt.jqgfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xqe.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://svf.zhaomingkeji.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cnt.jinghuilouyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://rgf.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jhg.redwolf501.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bkt.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://emk.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wxw.c1oappe.top

[L06] 解析响应为 JSON
来源：http://sjw.nanxuanxn.top

Py:   resp.json()
来源：http://tbp.cheryme.top

PHP:  json_decode($body, true);
来源：http://tqb.snrcjt.cn

JS:   await resp.json()
来源：http://ius.chenzaomai.com

TS:   await resp.json()
来源：http://bfg.guannengcc.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sib.ydjk.org.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zfh.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://hya.xziqi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://bwj.cashguo.top

[L07] 处理 HTTP 状态码
来源：http://pmx.fehbvm.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://tnp.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://emn.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://npv.zhiwuduotai.top

TS:   resp.ok;  resp.status
来源：http://xks.gaohongyu789.top

Java: resp.statusCode()
来源：http://ayl.smart0.xyz

Go:   resp.StatusCode
来源：http://pzj.uphjek.com

Ruby: resp.code.to_i
来源：http://ojb.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://rzv.sysykeji.top

[L08] 并发请求多个地址
来源：http://qfj.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ovc.jinqigfzy.top

PHP:  curl_multi_init() 系列
来源：http://fbx.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://erl.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bqe.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uer.haohaochexian.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lhu.yfazqb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jih.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://yqj.vehdjk.com

================================================================================
来源：http://skr.dianchejie.cn

M. 命令行 / 进程 / 环境
来源：http://ozn.shzxlz.cn

================================================================================
来源：http://che.xuanzx.com

[M01] 读取命令行参数
来源：http://oha.dashuyun.cn

Py:   sys.argv[1:]
来源：http://xnv.hywenlv.cn

PHP:  $argv;  $argc;
来源：http://iqz.ybcxt.top

JS:   process.argv.slice(2)
来源：http://ida.redwolf501.top

TS:   process.argv.slice(2)
来源：http://enm.yongpay.top

Java: args 数组（main 方法参数）
来源：http://cyr.ehwqpu.com

Go:   os.Args[1:]
来源：http://mzy.mhx1999.top

Ruby: ARGV
来源：http://rtn.yueranfly.top

C#:   args 数组（Main 方法参数）
来源：http://xog.shuidangran.top

[M02] 读取环境变量
来源：http://axe.pengpengdd.cyou

Py:   os.environ.get("HOME")
来源：http://erg.sysykeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rnb.fzhhl.top

JS:   process.env.HOME
来源：http://fqo.c1oappe.top

TS:   process.env.HOME
来源：http://afl.daxiang520.top

Java: System.getenv("HOME")
来源：http://lwo.yfazqb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rxm.jinghuilouyu.cn

Ruby: ENV["HOME"]
来源：http://yvz.xziqi.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tkg.uphjek.com

[M03] 执行外部命令
来源：http://blq.xingfuxueyuan.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wld.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://krh.zhixingplan.top

JS:   child_process.execSync("ls -l").toString()
来源：http://usn.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://sdf.zhijiandao.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zez.nanxuanxn.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mov.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qcq.hammf.cn

C#:   Process.Start("ls", "-l");
来源：http://hue.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://prb.yj202588.top

Py:   os.getcwd()
来源：http://qer.chenlongwang.top

PHP:  getcwd();
来源：http://lew.52xcode.cn

JS:   process.cwd()
来源：http://yjj.daria6918.cn

TS:   process.cwd()
来源：http://csb.cashguo.top

Java: Path.of("").toAbsolutePath()
来源：http://djg.dashuyun.cn

Go:   os.Getwd()
来源：http://fhz.yuxming.cn

Ruby: Dir.pwd
来源：http://bos.yongpay.top

C#:   Directory.GetCurrentDirectory()
来源：http://htw.fanxiaobao.xyz

[M05] 设置退出码
来源：http://xyi.jinqigufen.top

Py:   sys.exit(1)
来源：http://ljl.haohaochexian.top

PHP:  exit(1);
来源：http://blp.316326.xyz

JS:   process.exit(1)
来源：http://nbl.hcnkem.com

TS:   process.exit(1)
来源：http://mly.meibo888.top

Java: System.exit(1)
来源：http://xfp.zhixingplan.top

Go:   os.Exit(1)
来源：http://ope.havefunace.top

Ruby: exit 1
来源：http://jlr.hywenlv.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ihd.ywan-chungtsiang.top

[M06] 向标准错误输出
来源：http://dee.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://hom.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://olc.pengpengdd.cyou

JS:   console.error("err")
来源：http://asv.hysaishi.cn

TS:   console.error("err")
来源：http://skq.ppjwa.cn

Java: System.err.println("err")
来源：http://sqw.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xdr.zhaomingkeji.xyz

Ruby: warn "err"
来源：http://sut.kuanghao11.cn

C#:   Console.Error.WriteLine("err")
来源：http://hhj.zhongyouzk.top

[M07] 判断是否为主入口
来源：http://uwk.nanxinkj.top

Py:   if __name__ == "__main__":
来源：http://pvi.chenzaomai.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://qqm.sjlbkw.cn

JS:   require.main === module
来源：http://cde.yfazqb.com

TS:   require.main === module
来源：http://wmg.yangfankeji.com

Java: public static void main(String[] args)
来源：http://etk.ehwqpu.com

Go:   func main()
来源：http://wby.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ckj.chenzaomai.com

C#:   static void Main(string[] args)
来源：http://leu.yj20258888.top

[M08] 获取系统与运行时信息
来源：http://dsi.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://onn.zhongyouzk.top

PHP:  PHP_OS;  phpversion();
来源：http://vos.9152youxi.cn

JS:   process.platform;  process.version
来源：http://ikd.yfazqb.com

TS:   process.platform;  process.version
来源：http://qqu.redwolf501.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jmc.shzxlz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nim.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eug.xinyue.icu

C#:   Environment.OSVersion;  Environment.Version
来源：http://tgm.yanxiufei.cn

================================================================================
来源：http://ota.jinghuilouyu.cn

N. 数据结构与算法
来源：http://sza.ydzc1.top

================================================================================
来源：http://pys.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://bfu.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qdl.redwolf501.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mvv.wangshuangyany.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://udc.hfpthk.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wjy.ywan-chungtsiang.top

Java: Arrays.binarySearch(arr, x)
来源：http://rxv.chenjidiqi.icu

Go:   sort.SearchInts(arr, x)
来源：http://mra.shzxlz.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dsv.jinghuilouyu.cn

C#:   Array.BinarySearch(arr, x)
来源：http://njg.ydjk.org.cn

[N02] 排序（工程实践用内置实现）
来源：http://akw.gotoacloud.top

Py:   sorted(arr);  arr.sort()
来源：http://tgf.chenjidiqi.icu

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://keu.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://cxa.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://bqc.tanke756.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://chm.dashuyun.cn

Go:   slices.Sort(arr)
来源：http://eli.jinghuilouyu.cn

Ruby: arr.sort
来源：http://tzv.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://uvc.nwbrower.top

[N03] 快速排序（分治示例）
来源：http://oag.zdbjq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lnm.ydzc1.top

PHP:  // 递归实现，或用 usort
来源：http://kfe.ctjpmb.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://emh.yj202588.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://byc.cucudq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eil.smart0.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://uay.fzhhl.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://efc.pycfn.com

C#:   // 手写递归，或 Array.Sort
来源：http://jzc.gaohongyu789.top

[N04] 斐波那契数列
来源：http://pay.dashuyun.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fkf.zhongyouzk.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gvw.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nnr.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vhp.cashguo.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pur.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ous.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://uhq.c1oappe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dps.havefunace.top

[N05] 最大公约数
来源：http://wdu.birdmap.top

Py:   math.gcd(a, b)
来源：http://fsd.fehbvm.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cvn.shanyushiyangkeji.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fza.fengsongda.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://brh.guowangkeji.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vna.sufxvd.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://kti.cashguo.top

Ruby: a.gcd(b)
来源：http://num.hammf.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dwo.cheryme.top

[N06] 判断回文字符串
来源：http://qzr.ivvv.top

Py:   s == s[::-1]
来源：http://qel.ctjpmb.com

PHP:  $s === strrev($s);
来源：http://uuq.xuetiantiany.cn

JS:   s === [...s].reverse().join("")
来源：http://rus.daria6918.cn

TS:   s === [...s].reverse().join("")
来源：http://upe.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fim.cdnleiting.top

Go:   // 双指针从两端比较
来源：http://pdw.fktsv.cn

Ruby: s == s.reverse
来源：http://xwx.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://upb.yfazqb.com

[N07] 两数之和（返回下标）
来源：http://uul.316326.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zsd.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://peh.shanyushiyangtech.top

JS:   // 手写 Map：map.set(v, i)
来源：http://joh.sysykeji.top

TS:   // 手写 Map<string, number>
来源：http://hil.ctjpmb.com

Java: // 手写 HashMap
来源：http://zyd.daria6918.cn

Go:   // 手写 map[int]int
来源：http://net.dianchejie.cn

Ruby: // 手写 Hash
来源：http://kck.zdqjudy.top

C#:   // 手写 Dictionary<int, int>
来源：http://mwh.cashguo.top

[N08] 生成全排列
来源：http://meq.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://weh.hnqzz.top

PHP:  // 手写递归交换
来源：http://vas.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://gcz.zdqjudy.top

TS:   // 手写回溯递归
来源：http://jmw.fehbvm.com

Java: // 手写回溯递归
来源：http://lsp.guowangkeji.top

Go:   // 手写回溯递归
来源：http://mfi.xuanzx.com

Ruby: arr.permutation.to_a
来源：http://cvq.yonumen.top

C#:   // 手写回溯递归
来源：http://ofs.jlsjyb.cn

[N09] 栈与队列
来源：http://jcz.zdbjq.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://suy.daxiang520.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://jef.xinyue.icu

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://nkg.dianchejie.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bif.ydjk.org.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://fcx.xylfe.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://eqf.cqqwz.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://xba.chenlongwang.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://afq.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://bna.chenjidiqi.icu

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://igv.tarul.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://ofd.hongshengwenyu.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://hqs.yanxiufei.cn

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://lqg.smart0.xyz

Java: class Node { int v; Node next; }
来源：http://jrk.c1oappe.top

Go:   type Node struct { V int; Next *Node }
来源：http://ymz.meibo888.top

Ruby: Node = Struct.new(:v, :next)
来源：http://nex.ppjwa.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://wmw.yuanzhike.top

[N11] 二叉树中序遍历
来源：http://yda.zhaomingkeji.xyz

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://edw.ywan-chungtsiang.top

PHP:  // 手写递归函数
来源：http://yqp.zhoulong.xyz

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://xag.sxryk.cn

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://cwv.ydjk.org.cn

Java: // 手写递归
来源：http://wpf.hywenlv.cn

Go:   // 手写递归
来源：http://aji.tanke756.top

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://yta.nwbrower.top

C#:   // 手写递归
来源：http://uuf.redwolf501.top

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://zdh.uphjek.com

Py:   from functools import reduce;  climb = lambda n: reduce(lambda p, _: (p[1], p[0] + p[1]), range(n), (1, 1))[0]
来源：http://mhf.kuanghao11.cn

PHP:  // 递推：$a=1;$b=1;for(...){[$a,$b]=[$b,$a+$b];}
来源：http://kmx.fehbvm.com

JS:   // 递推：let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://iqd.xuetiantiany.cn

TS:   let [a, b] = [1, 1]; for (let i = 0; i < n; i++) [a, b] = [b, a + b];
来源：http://zrv.yuxming.cn

Java: // 递推：int a = 1, b = 1; 循环更新
来源：http://juj.zdqjudy.top

Go:   // 递推：a, b := 1, 1; for i := 0; i < n; i++ { a, b = b, a+b }
来源：http://hgm.xylfe.cn

Ruby: a, b = 1, 1;  n.times { a, b = b, a + b }
来源：http://vnj.cdnleiting.top

C#:   // 递推：int a = 1, b = 1; 循环更新
来源：http://rau.zhaomingkeji.xyz

================================================================================
来源：http://vmz.andypj.xyz

O. 并发与异步
来源：http://msz.shanyushiyangtech.top

================================================================================
来源：http://lab.smart0.xyz

[O01] 启动一个线程
来源：http://rtk.zdqjudy.top

Py:   threading.Thread(target=f, args=(1,)).start()
来源：http://tfm.ybcxt.top

PHP:  // 无原生线程：用 pcntl_fork 或消息队列
来源：http://qyg.yonumen.top

JS:   // 单线程事件循环：CPU 密集用 worker_threads
来源：http://hid.snrcjt.cn

TS:   // 同 JS
来源：http://wgp.uphjek.com

Java: new Thread(() -> f()).start()
来源：http://laf.nanxuanxn.top

Go:   go f()
来源：http://nbv.xziqi.cn

Ruby: Thread.new { f }
来源：http://fsa.sysykeji.top

C#:   Task.Run(() => F());
来源：http://hzx.yanxiufei.cn


<!-- 参考信息 -->