代发 wailian999

Ruby: JSON.pretty_generate(obj)
来源：http://wec.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xpl.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://opd.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hnz.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uql.tanke756.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gqe.guannengcc.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bkw.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gug.aizwys.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kov.jianghu66.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jgf.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uid.svipenyu.cn

[K05] 深拷贝对象
来源：http://rnk.fanxiaobao.xyz

Py:   copy.deepcopy(obj)
来源：http://dpq.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://pfg.mhx1999.top

JS:   structuredClone(obj)
来源：http://jjx.tian-w.cn

TS:   structuredClone(obj)
来源：http://pkk.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://ikd.jianghu66.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gwb.yuxming.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hri.tianlin.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://qhy.jinyuanbaomall.cn

[K06] 解析 URL 查询串
来源：http://jcv.jinqigufen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hng.zhoulong.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yqw.jianghu66.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bda.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kni.zhaomingkeji.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dis.ywan-chungtsiang.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tcy.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ewm.gzhubu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://udq.yvedp.cn

[K07] 进制转换
来源：http://lgu.sjlbkw.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ede.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tvi.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zfx.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://yll.yongpay.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tey.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vus.cdnleiting.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yoq.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://cyg.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://gyg.shangyingyoupin.top

Py:   pickle.dumps(obj)
来源：http://him.0kj1m.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yhb.ydjk.org.cn

JS:   v8.serialize(obj)        // Node
来源：http://qzt.jianghu66.top

TS:   v8.serialize(obj)        // Node
来源：http://dax.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zfz.zycfv.cn

Go:   encoding/gob
来源：http://fvo.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://ijp.ivvv.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mzf.xuetiantiany.cn

================================================================================
来源：http://yme.tarul.cn

L. 网络请求
来源：http://xwj.chenlongwang.top

================================================================================
来源：http://xbs.jqgufenzy.top

[L01] 发送 GET 请求
来源：http://bms.yuanzhike.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vnu.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://vdk.xinyue.icu

JS:   await fetch(url)
来源：http://plu.shanyushiyangtech.top

TS:   await fetch(url)
来源：http://myh.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://edv.hnxiangtu.top

Go:   resp, err := http.Get(url)
来源：http://oxw.pengpengdd.cyou

Ruby: Net::HTTP.get(URI(url))
来源：http://cwl.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dth.zhixingplan.top

[L02] 发送 POST JSON
来源：http://lbu.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://qjr.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qay.cqqwz.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uaq.tianlin.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ziu.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jda.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rdc.dashuyun.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ybj.cqqwz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pjr.bbcook.cn

[L03] 设置自定义请求头
来源：http://gfx.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://uwb.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ckj.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aqi.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nii.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wce.nwbrower.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sgz.yj202588.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cng.sjlbkw.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://one.vqdsnc.cn

[L04] 设置超时
来源：http://ski.cashguo.top

Py:   requests.get(url, timeout=5)
来源：http://usw.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fde.daxiang520.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lda.jinqigufen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jtz.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ljx.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qvx.yangfankeji.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rgv.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gnj.fehbvm.com

[L05] 上传文件（multipart）
来源：http://ibv.andypj.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://evs.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tpl.shangyingyoupin.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tdr.ivvv.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tdh.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jbr.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ydi.nanxuanxn.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://att.ydzc1.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dbj.cashguo.top

[L06] 解析响应为 JSON
来源：http://can.jqgufenzy.top

Py:   resp.json()
来源：http://nmh.hnxiangtu.top

PHP:  json_decode($body, true);
来源：http://njd.epnwcf.com

JS:   await resp.json()
来源：http://gig.guowangkeji.top

TS:   await resp.json()
来源：http://xji.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nhn.sysykeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uuf.guowangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://uiy.cucudq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://thv.andypj.xyz

[L07] 处理 HTTP 状态码
来源：http://cca.sysykeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ovl.yonumen.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xfs.nanxuanxn.top

JS:   resp.ok;  resp.status
来源：http://pfg.pengpengdd.cyou

TS:   resp.ok;  resp.status
来源：http://brz.vqdsnc.cn

Java: resp.statusCode()
来源：http://dcj.ybcxt.top

Go:   resp.StatusCode
来源：http://lrp.sysykeji.top

Ruby: resp.code.to_i
来源：http://ttl.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://bre.haohaochexian.top

[L08] 并发请求多个地址
来源：http://dtq.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dnr.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://wjk.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tno.shuidangran.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zec.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rga.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://rmq.zhengqikj.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://edo.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://coj.jiagoushi.top

================================================================================
来源：http://akn.zhixingplan.top

M. 命令行 / 进程 / 环境
来源：http://lym.daria6918.cn

================================================================================
来源：http://fcg.andypj.xyz

[M01] 读取命令行参数
来源：http://egf.uphjek.com

Py:   sys.argv[1:]
来源：http://bpj.xziqi.cn

PHP:  $argv;  $argc;
来源：http://ioi.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://lrb.nanxuanxn.top

TS:   process.argv.slice(2)
来源：http://pic.yangfankeji.com

Java: args 数组（main 方法参数）
来源：http://ohp.bjfxy.top

Go:   os.Args[1:]
来源：http://ugz.hcnkem.com

Ruby: ARGV
来源：http://pxp.jyoumei.cn

C#:   args 数组（Main 方法参数）
来源：http://coz.nanxinkj.top

[M02] 读取环境变量
来源：http://bcb.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://qjg.xuanzx.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jfe.yj20258888.top

JS:   process.env.HOME
来源：http://qtr.xinyue.icu

TS:   process.env.HOME
来源：http://ydl.bbcook.cn

Java: System.getenv("HOME")
来源：http://oud.tarul.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rit.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://hcy.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://aqo.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://sst.sysykeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fat.sjlbkw.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lim.zhaomingkeji.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://ydt.cucudq.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ouu.zhijiandao.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uho.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gzs.zhongyouzk.top

Ruby: system("ls -l");  `ls -l`
来源：http://zlz.havefunace.top

C#:   Process.Start("ls", "-l");
来源：http://zor.epnwcf.com

[M04] 获取当前工作目录
来源：http://fpf.andypj.xyz

Py:   os.getcwd()
来源：http://xtz.fanxiaobao.xyz

PHP:  getcwd();
来源：http://pib.cucudq.cn

JS:   process.cwd()
来源：http://bnd.cdnleiting.top

TS:   process.cwd()
来源：http://bbh.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://zbl.uphjek.com

Go:   os.Getwd()
来源：http://mup.hammf.cn

Ruby: Dir.pwd
来源：http://nya.ppjwa.cn

C#:   Directory.GetCurrentDirectory()
来源：http://frb.ydjk.org.cn

[M05] 设置退出码
来源：http://ydf.cucudq.cn

Py:   sys.exit(1)
来源：http://let.shanyushiyangtech.top

PHP:  exit(1);
来源：http://gvy.cdnleiting.top

JS:   process.exit(1)
来源：http://dad.316326.xyz

TS:   process.exit(1)
来源：http://gjx.wangdashe.top

Java: System.exit(1)
来源：http://ymt.hesvh.cn

Go:   os.Exit(1)
来源：http://fgp.zhijiandao.cn

Ruby: exit 1
来源：http://mij.jqgufenzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://foe.fanxiaobao.xyz

[M06] 向标准错误输出
来源：http://ukn.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://wvp.yuxming.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xtb.zhengqikj.top

JS:   console.error("err")
来源：http://cor.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://dpt.redwolf501.top

Java: System.err.println("err")
来源：http://duz.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gwn.mhx1999.top

Ruby: warn "err"
来源：http://rpa.birdmap.top

C#:   Console.Error.WriteLine("err")
来源：http://sso.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://dlj.ybcxt.top

Py:   if __name__ == "__main__":
来源：http://qff.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lsk.havefunace.top

JS:   require.main === module
来源：http://eid.svipenyu.cn

TS:   require.main === module
来源：http://edi.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://opm.xziqi.cn

Go:   func main()
来源：http://iqn.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nzb.0kj1m.cn

C#:   static void Main(string[] args)
来源：http://pkj.wangdashe.top

[M08] 获取系统与运行时信息
来源：http://akm.gotoacloud.top

Py:   platform.system();  platform.python_version()
来源：http://hbz.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://jzo.zhongyouzk.top

JS:   process.platform;  process.version
来源：http://gbb.yj202588.top

TS:   process.platform;  process.version
来源：http://vgf.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://lmc.feifeiyinyue.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tnu.fengsongda.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ssn.pycfn.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://qzt.meibo888.top

================================================================================
来源：http://wrf.nanxuanxn.top

N. 数据结构与算法
来源：http://gev.ehwqpu.com

================================================================================
来源：http://qtb.bjfxy.top

[N01] 二分查找（有序数组）
来源：http://dhh.fengsongda.top

Py:   bisect.bisect_left(arr, x)
来源：http://pxa.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jay.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ggy.jinqigfzy.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wss.sysykeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://oxl.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://wxp.hongshengwenyu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://mgc.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://mpy.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://obr.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://cno.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pcw.yuxming.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dbx.nanxuanxn.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://drv.hongshengwenyu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lfd.hongshengwenyu.top

Go:   slices.Sort(arr)
来源：http://ryq.aizwys.cn

Ruby: arr.sort
来源：http://shu.fktsv.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mqz.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://urc.ivvv.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ufk.cqqwz.cn

PHP:  // 递归实现，或用 usort
来源：http://hwp.smart0.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uvq.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://bmz.hnxiangtu.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vaq.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gwj.jinyuanbaomall.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vgv.jianghu66.top

C#:   // 手写递归，或 Array.Sort
来源：http://vsj.yvedp.cn

[N04] 斐波那契数列
来源：http://yqm.xziqi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xgq.vehdjk.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fyv.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nyi.shzxlz.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bpu.daria6918.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wso.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mxa.ehwqpu.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qzi.ivvv.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cir.xziqi.cn

[N05] 最大公约数
来源：http://koa.xylfe.cn

Py:   math.gcd(a, b)
来源：http://yfy.tianlin.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jqj.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tby.c1oappe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fxb.yangfankeji.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://tdg.wangdashe.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cux.hfpthk.cn

Ruby: a.gcd(b)
来源：http://uet.mhx1999.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://icq.zhongyouzk.top

[N06] 判断回文字符串
来源：http://psw.gotoacloud.top

Py:   s == s[::-1]
来源：http://yhs.daria6918.cn

PHP:  $s === strrev($s);
来源：http://owz.andypj.xyz

JS:   s === [...s].reverse().join("")
来源：http://qhv.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://wjo.cheryme.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ncq.birdmap.top

Go:   // 双指针从两端比较
来源：http://rlp.aibaodan.cn

Ruby: s == s.reverse
来源：http://ugb.zhengqikj.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bnx.guowangkeji.top

[N07] 两数之和（返回下标）
来源：http://ran.kuanghao11.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sle.yanxiufei.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://hqp.yvedp.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://pbm.yuanzhike.top

TS:   // 手写 Map<string, number>
来源：http://cjs.daxiang520.top

Java: // 手写 HashMap
来源：http://swd.tarul.cn

Go:   // 手写 map[int]int
来源：http://kcr.andypj.xyz

Ruby: // 手写 Hash
来源：http://tbf.hywenlv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://zqb.ydzc1.top

[N08] 生成全排列
来源：http://qmg.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://tgm.sxryk.cn

PHP:  // 手写递归交换
来源：http://rgv.shzxlz.cn

JS:   // 手写回溯递归
来源：http://suk.yj20258.top

TS:   // 手写回溯递归
来源：http://ofj.haohaochexian.top

Java: // 手写回溯递归
来源：http://txp.xuanzx.com

Go:   // 手写回溯递归
来源：http://dgi.52xcode.cn

Ruby: arr.permutation.to_a
来源：http://lod.smart0.xyz

C#:   // 手写回溯递归
来源：http://zut.zhijiandao.cn

[N09] 栈与队列
来源：http://kws.fehbvm.com

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://imn.sjlbkw.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://axy.snrcjt.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://sbs.sweek.top

TS:   arr.push(x) / arr.pop() 作栈
来源：http://bhd.bjfxy.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://tly.hysaishi.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://mcb.ppjwa.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://iqq.yonumen.top

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://jmg.fanxiaobao.xyz

[N10] 链表节点定义
来源：http://blo.c1oappe.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://bel.yj202588.top

PHP:  class Node { public $v; public $next = null; }
来源：http://yzs.shanyushiyangkeji.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://xjb.cashguo.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://hgq.hysaishi.cn

Java: class Node { int v; Node next; }
来源：http://slh.haohaochexian.top

Go:   type Node struct { V int; Next *Node }
来源：http://xlw.shangyingyoupin.top

Ruby: Node = Struct.new(:v, :next)
来源：http://tmw.hywenlv.cn

C#:   class Node { public int V; public Node? Next; }
来源：http://ljl.shuidangran.top

[N11] 二叉树中序遍历
来源：http://axc.daria6918.cn

Py:   def inorder(n): return inorder(n.left) + [n.val] + inorder(n.right) if n else []
来源：http://vgl.redwolf501.top

PHP:  // 手写递归函数
来源：http://zyy.hywenlv.cn

JS:   const inorder = n => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://moq.hcnkem.com

TS:   const inorder = (n: T | null): number[] => n ? [...inorder(n.left), n.val, ...inorder(n.right)] : [];
来源：http://mol.hammf.cn

Java: // 手写递归
来源：http://foo.cucudq.cn

Go:   // 手写递归
来源：http://dkf.52xcode.cn

Ruby: def inorder(n) = n ? inorder(n.left) + [n.val] + inorder(n.right) : []
来源：http://frq.redwolf501.top

C#:   // 手写递归
来源：http://btl.chenjidiqi.icu

[N12] 动态规划：爬楼梯（每次 1 或 2 级）
来源：http://mjs.tarul.cn


<!-- 参考信息 -->