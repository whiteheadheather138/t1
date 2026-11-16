代发 wailian999

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zpk.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://msz.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://jim.yj202588.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hup.yangfankeji.com

JS:   JSON.stringify(obj, null, 2)
来源：http://laj.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://lwr.shanyushiyangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rmn.shanyushiyangtech.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://flq.yvedp.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gfk.tanke756.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wxm.tarul.cn

[K04] 读取 JSON 文件
来源：http://ook.zhongyouzk.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gzb.jianghu66.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mic.uphjek.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zcq.sweek.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://god.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://tuo.iojbl.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fmd.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://kgq.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tau.yj20258.top

[K05] 深拷贝对象
来源：http://pil.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://lpo.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://biu.hfpthk.cn

JS:   structuredClone(obj)
来源：http://cgw.zhengqikj.top

TS:   structuredClone(obj)
来源：http://bgl.jlsjyb.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://upf.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://rbp.nanxinkj.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://shv.xingfuxueyuan.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://ltn.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://eyp.shuidangran.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lal.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zdc.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nue.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jzn.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://any.xingfuxueyuan.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://exw.tanke756.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://chn.sxryk.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://org.nwbrower.top

[K07] 进制转换
来源：http://chr.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hmh.havefunace.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://der.hysaishi.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tat.jiagoushi.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://exc.shanyushiyangtech.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ujm.sxryk.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gse.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://qhv.smart0.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rnn.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://fac.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://dbt.cheryme.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dss.jqgfzy.top

JS:   v8.serialize(obj)        // Node
来源：http://iqc.shanyushiyangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://vxf.gaohongyu789.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zdi.andypj.xyz

Go:   encoding/gob
来源：http://kmr.vehdjk.com

Ruby: Marshal.dump(obj)
来源：http://ybc.bjfxy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ous.c1oappe.top

================================================================================
来源：http://ykn.feifeiyinyue.top

L. 网络请求
来源：http://cqv.jinqigufen.top

================================================================================
来源：http://ckj.yonumen.top

[L01] 发送 GET 请求
来源：http://yjd.yueranfly.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xiy.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fba.hcnkem.com

JS:   await fetch(url)
来源：http://uqq.xinyue.icu

TS:   await fetch(url)
来源：http://gee.quarkkingdee.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://biu.dianchejie.cn

Go:   resp, err := http.Get(url)
来源：http://fza.sweek.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qep.gzhubu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://huh.shangyingyoupin.top

[L02] 发送 POST JSON
来源：http://ixh.andypj.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://ncw.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tgo.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mae.yuanzhike.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nxx.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uuh.shangyingyoupin.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mlm.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qvz.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ssi.svipenyu.cn

[L03] 设置自定义请求头
来源：http://rgz.zhixingplan.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yrt.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://igb.dashuyun.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dic.hongshengwenyu.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jgp.jinghuilouyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pux.mhx1999.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eoo.52xcode.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://qej.hammf.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qxm.kuanghao11.cn

[L04] 设置超时
来源：http://bir.gotoacloud.top

Py:   requests.get(url, timeout=5)
来源：http://ytm.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://jkm.feifeiyinyue.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ldm.316326.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ngf.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qtn.guannengcc.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mga.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://edi.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pbm.iojbl.cn

[L05] 上传文件（multipart）
来源：http://kmr.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wky.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tsm.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uft.yuanzhike.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yuf.cashguo.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fgy.c1oappe.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ppr.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://sle.jinqigfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mnw.nanxuanxn.top

[L06] 解析响应为 JSON
来源：http://tny.tian-w.cn

Py:   resp.json()
来源：http://ccb.tianlin.xyz

PHP:  json_decode($body, true);
来源：http://fjy.0kj1m.cn

JS:   await resp.json()
来源：http://jmv.zhengqikj.top

TS:   await resp.json()
来源：http://xih.sjlbkw.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://znn.zhixingplan.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ftn.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://shv.jianghu66.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fnx.nwbrower.top

[L07] 处理 HTTP 状态码
来源：http://fuu.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://brz.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://cji.haohaochexian.top

JS:   resp.ok;  resp.status
来源：http://jyi.daria6918.cn

TS:   resp.ok;  resp.status
来源：http://zvs.chenjidiqi.icu

Java: resp.statusCode()
来源：http://hxr.yongpay.top

Go:   resp.StatusCode
来源：http://dpj.xuanzx.com

Ruby: resp.code.to_i
来源：http://bng.jinqigufen.top

C#:   (int)resp.StatusCode
来源：http://ldq.guowangkeji.top

[L08] 并发请求多个地址
来源：http://fgz.cashguo.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mpm.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://nmx.zdbjq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kyp.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yer.hammf.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nrg.jinyuanbaomall.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://kww.ppjwa.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://abv.meibo888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ukf.redwolf501.top

================================================================================
来源：http://xuw.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://uen.dashuyun.cn

================================================================================
来源：http://bom.nanxuanxn.top

[M01] 读取命令行参数
来源：http://csz.jinqigufen.top

Py:   sys.argv[1:]
来源：http://sfi.fanxiaobao.xyz

PHP:  $argv;  $argc;
来源：http://kjr.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://cuu.shzxlz.cn

TS:   process.argv.slice(2)
来源：http://whv.dashuyun.cn

Java: args 数组（main 方法参数）
来源：http://qmh.chenlongwang.top

Go:   os.Args[1:]
来源：http://pfr.yongpay.top

Ruby: ARGV
来源：http://vub.cucudq.cn

C#:   args 数组（Main 方法参数）
来源：http://lsi.ctjpmb.com

[M02] 读取环境变量
来源：http://fap.feifeiyinyue.top

Py:   os.environ.get("HOME")
来源：http://hil.birdmap.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://awj.fehbvm.com

JS:   process.env.HOME
来源：http://rmk.yonumen.top

TS:   process.env.HOME
来源：http://rno.quarkkingdee.top

Java: System.getenv("HOME")
来源：http://goh.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cei.hnxiangtu.top

Ruby: ENV["HOME"]
来源：http://wch.dianchejie.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kwd.mhx1999.top

[M03] 执行外部命令
来源：http://etj.zhengqikj.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://roi.aizwys.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ywd.sysykeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bil.yangfankeji.com

TS:   child_process.execSync("ls -l").toString()
来源：http://wmb.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://qps.redwolf501.top

Go:   exec.Command("ls", "-l").Output()
来源：http://fyw.gaohongyu789.top

Ruby: system("ls -l");  `ls -l`
来源：http://qom.mhx1999.top

C#:   Process.Start("ls", "-l");
来源：http://vgw.cdnleiting.top

[M04] 获取当前工作目录
来源：http://ufc.zhijiandao.cn

Py:   os.getcwd()
来源：http://nzx.cashguo.top

PHP:  getcwd();
来源：http://qrr.fanxiaobao.xyz

JS:   process.cwd()
来源：http://pai.wangdashe.top

TS:   process.cwd()
来源：http://uxw.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://mup.quarkkingdee.top

Go:   os.Getwd()
来源：http://neb.zdbjq.cn

Ruby: Dir.pwd
来源：http://pct.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://bgk.cheryme.top

[M05] 设置退出码
来源：http://tjb.yj20258888.top

Py:   sys.exit(1)
来源：http://lsi.hongshengwenyu.top

PHP:  exit(1);
来源：http://mpr.cucudq.cn

JS:   process.exit(1)
来源：http://cun.havefunace.top

TS:   process.exit(1)
来源：http://ukf.uphjek.com

Java: System.exit(1)
来源：http://hmd.cdnleiting.top

Go:   os.Exit(1)
来源：http://xfa.chenjidiqi.icu

Ruby: exit 1
来源：http://rxa.aizwys.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lna.wangdashe.top

[M06] 向标准错误输出
来源：http://qlv.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://oqi.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://flo.yonumen.top

JS:   console.error("err")
来源：http://qpj.nwbrower.top

TS:   console.error("err")
来源：http://tyz.gotoacloud.top

Java: System.err.println("err")
来源：http://nkc.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lsx.nanxuanxn.top

Ruby: warn "err"
来源：http://cqh.meibo888.top

C#:   Console.Error.WriteLine("err")
来源：http://tho.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://hfr.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://enc.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oci.hywenlv.cn

JS:   require.main === module
来源：http://xne.zhengqikj.top

TS:   require.main === module
来源：http://qmu.zhongyouzk.top

Java: public static void main(String[] args)
来源：http://cig.ydzc1.top

Go:   func main()
来源：http://wbw.shangyingyoupin.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://css.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://wip.zhongyouzk.top

[M08] 获取系统与运行时信息
来源：http://ctd.ybcxt.top

Py:   platform.system();  platform.python_version()
来源：http://atr.yongpay.top

PHP:  PHP_OS;  phpversion();
来源：http://pma.xinyue.icu

JS:   process.platform;  process.version
来源：http://iyo.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://gsa.ivvv.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fyr.wangdashe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://nei.pengpengdd.cyou

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tgk.tanke756.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://xop.9152youxi.cn

================================================================================
来源：http://wpw.dianchejie.cn

N. 数据结构与算法
来源：http://ulb.birdmap.top

================================================================================
来源：http://niu.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://bjm.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://yms.jinqigufen.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://sup.pycfn.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://opn.gogol.net.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wkw.cdnleiting.top

Java: Arrays.binarySearch(arr, x)
来源：http://vbe.smart0.xyz

Go:   sort.SearchInts(arr, x)
来源：http://txw.guannengcc.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rzy.shzxlz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://stv.shangyingyoupin.top

[N02] 排序（工程实践用内置实现）
来源：http://zts.shzxlz.cn

Py:   sorted(arr);  arr.sort()
来源：http://trr.yfazqb.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lop.aizwys.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ppu.haohaochexian.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cye.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xpu.andypj.xyz

Go:   slices.Sort(arr)
来源：http://otj.zhiwuduotai.top

Ruby: arr.sort
来源：http://aac.shanyushiyangtech.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://hza.chenjidiqi.icu

[N03] 快速排序（分治示例）
来源：http://sxu.birdmap.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wiw.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://cjq.52xcode.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qat.bbcook.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ilf.tian-w.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://efj.shuidangran.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://izw.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ruf.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hoz.zhixingplan.top

[N04] 斐波那契数列
来源：http://wjr.yueranfly.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gup.c1oappe.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zfi.sxryk.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jnl.jqgfzy.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uvl.yonumen.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cim.xingfuxueyuan.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ypq.fktsv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://twg.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dri.dianchejie.cn

[N05] 最大公约数
来源：http://ocn.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://wsx.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lax.zycfv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://knt.vehdjk.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nxy.svipenyu.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uob.jinyuanbaomall.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ypl.hcnkem.com

Ruby: a.gcd(b)
来源：http://tmo.ehwqpu.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://zsi.52xcode.cn

[N06] 判断回文字符串
来源：http://fiu.haohaochexian.top

Py:   s == s[::-1]
来源：http://lre.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://anv.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://nbq.zhoulong.xyz

TS:   s === [...s].reverse().join("")
来源：http://arb.zdbjq.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://akl.xinyue.icu

Go:   // 双指针从两端比较
来源：http://fml.feifeiyinyue.top

Ruby: s == s.reverse
来源：http://yye.yanxiufei.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ein.fehbvm.com

[N07] 两数之和（返回下标）
来源：http://ouh.fehbvm.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://imd.fzhhl.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nxs.jqgufenzy.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ven.gogol.net.cn

TS:   // 手写 Map<string, number>
来源：http://cia.ydjk.org.cn

Java: // 手写 HashMap
来源：http://ctx.vqdsnc.cn

Go:   // 手写 map[int]int
来源：http://gdx.zhoulong.xyz

Ruby: // 手写 Hash
来源：http://faa.jqgfzy.top

C#:   // 手写 Dictionary<int, int>
来源：http://qya.jinyuanbaomall.cn

[N08] 生成全排列
来源：http://ixo.nwbrower.top

Py:   itertools.permutations(arr)
来源：http://ush.haohaochexian.top

PHP:  // 手写递归交换
来源：http://dgf.sufxvd.cn

JS:   // 手写回溯递归
来源：http://tsl.zhengqikj.top

TS:   // 手写回溯递归
来源：http://vzb.nanxuanxn.top

Java: // 手写回溯递归
来源：http://myk.smart0.xyz

Go:   // 手写回溯递归
来源：http://knq.zhixingplan.top

Ruby: arr.permutation.to_a
来源：http://bbx.smart0.xyz

C#:   // 手写回溯递归
来源：http://asg.iojbl.cn

[N09] 栈与队列
来源：http://ail.xziqi.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://hme.chenjidiqi.icu

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://nhy.yonumen.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tvr.yonumen.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://dje.wangshuangyany.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://sev.yueranfly.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://khu.yfazqb.com

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://vkt.sysykeji.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://moq.shanyushiyangtech.top

[N10] 链表节点定义
来源：http://krp.bbcook.cn

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://arf.wangdashe.top

PHP:  class Node { public $v; public $next = null; }
来源：http://xio.zhaomingkeji.xyz

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://nao.hongshengwenyu.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ppv.zhijiandao.cn

Java: class Node { int v; Node next; }
来源：http://tif.gzhubu.top

Go:   type Node struct { V int; Next *Node }
来源：http://aqb.316326.xyz

Ruby: Node = Struct.new(:v, :next)
来源：http://ggk.sjlbkw.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://drb.tarul.cn

[N11] 二叉树中序遍历
来源：http://eqi.haohaochexian.top

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://evj.0kj1m.cn


<!-- 参考信息 -->