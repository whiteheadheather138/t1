代发 wailian999

TS:   JSON.parse(s)
来源：http://twj.yvedp.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://emk.jinyuanbaomall.cn

Go:   json.Unmarshal(data, &v)
来源：http://nkc.hnxiangtu.top

Ruby: JSON.parse(s)
来源：http://hai.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wbw.hnqzz.top

[K03] JSON 美化输出（带缩进）
来源：http://wbh.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vxh.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pbj.fengsongda.top

JS:   JSON.stringify(obj, null, 2)
来源：http://thh.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://khq.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://odt.ppjwa.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gxv.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://vlt.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pfs.pycfn.com

[K04] 读取 JSON 文件
来源：http://kpj.wangdashe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://far.sxryk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lnc.ehwqpu.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mzd.316326.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nmv.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fqd.dashuyun.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dnt.gogol.net.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://usk.sysykeji.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://kiv.bbcook.cn

[K05] 深拷贝对象
来源：http://utm.yvedp.cn

Py:   copy.deepcopy(obj)
来源：http://sbw.fehbvm.com

PHP:  unserialize(serialize($obj));
来源：http://xqk.sxryk.cn

JS:   structuredClone(obj)
来源：http://fou.xylfe.cn

TS:   structuredClone(obj)
来源：http://yza.fzhhl.top

Java: // 手写拷贝构造，或序列化往返
来源：http://eek.guowangkeji.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qye.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://agk.dashuyun.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://hlk.daxiang520.top

[K06] 解析 URL 查询串
来源：http://rvm.yongpay.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zzk.vqdsnc.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tsl.nwbrower.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://twd.meibo888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rfj.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://afo.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://eey.ydjk.org.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yuu.shangyingyoupin.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mvs.tarul.cn

[K07] 进制转换
来源：http://wki.ppjwa.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wyf.52xcode.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xie.hnxiangtu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jfa.hcnkem.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xuj.ehwqpu.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gtr.yj202588.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zrp.yongpay.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://itc.gaohongyu789.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ymp.zhongyouzk.top

[K08] 二进制序列化（非 JSON）
来源：http://jbv.guowangkeji.top

Py:   pickle.dumps(obj)
来源：http://dlq.chenjidiqi.icu

PHP:  serialize($obj);  unserialize($s);
来源：http://cgv.jlsjyb.cn

JS:   v8.serialize(obj)        // Node
来源：http://vje.jinqigufen.top

TS:   v8.serialize(obj)        // Node
来源：http://opi.xuetiantiany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dpa.jiagoushi.top

Go:   encoding/gob
来源：http://mfx.ppjwa.cn

Ruby: Marshal.dump(obj)
来源：http://lnz.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://csd.ivvv.top

================================================================================
来源：http://duq.aibaodan.cn

L. 网络请求
来源：http://dxx.redwolf501.top

================================================================================
来源：http://fyy.ydzc1.top

[L01] 发送 GET 请求
来源：http://cqs.xuetiantiany.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vcj.ybcxt.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://krg.hcnkem.com

JS:   await fetch(url)
来源：http://rai.birdmap.top

TS:   await fetch(url)
来源：http://kdt.jinqigufen.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gkp.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://now.jinqigfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ewr.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gfx.ywan-chungtsiang.top

[L02] 发送 POST JSON
来源：http://oqv.fzhhl.top

Py:   requests.post(url, json={"a": 1})
来源：http://spi.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ieh.yfazqb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xzu.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lxr.guowangkeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qcz.gogol.net.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kmx.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ywa.aibaodan.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uvw.hesvh.cn

[L03] 设置自定义请求头
来源：http://xfr.shanyushiyangtech.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jfv.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mme.hnxiangtu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sal.tarul.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ieb.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wxj.chenlongwang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tot.316326.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ibc.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://foa.jlsjyb.cn

[L04] 设置超时
来源：http://irn.kuanghao11.cn

Py:   requests.get(url, timeout=5)
来源：http://dtg.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rzs.vqdsnc.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://pdu.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wxg.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wtc.zhijiandao.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://juu.yuanzhike.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sal.iojbl.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ssp.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://azx.snrcjt.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://qjn.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ywj.pengpengdd.cyou

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://adc.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gjr.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://scm.xingfuxueyuan.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tso.zhoulong.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mbw.9152youxi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fwc.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://uzn.feifeiyinyue.top

Py:   resp.json()
来源：http://yxo.xziqi.cn

PHP:  json_decode($body, true);
来源：http://slv.fanxiaobao.xyz

JS:   await resp.json()
来源：http://lzk.ctjpmb.com

TS:   await resp.json()
来源：http://qeq.yuanzhike.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dbp.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ahi.bbcook.cn

Ruby: JSON.parse(resp.body)
来源：http://drg.svipenyu.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://odu.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://njs.yuanzhike.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sok.zhongyouzk.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://grl.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://wdq.jiagoushi.top

TS:   resp.ok;  resp.status
来源：http://ipl.bbcook.cn

Java: resp.statusCode()
来源：http://icg.jinqigufen.top

Go:   resp.StatusCode
来源：http://sch.yj20258888.top

Ruby: resp.code.to_i
来源：http://rql.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://egt.cheryme.top

[L08] 并发请求多个地址
来源：http://zde.daxiang520.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rjd.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://htp.zhoulong.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bzm.kuanghao11.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://php.hnxiangtu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ujw.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://reu.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ibo.andypj.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sek.mhx1999.top

================================================================================
来源：http://lik.uphjek.com

M. 命令行 / 进程 / 环境
来源：http://mnk.yanxiufei.cn

================================================================================
来源：http://vvn.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://hge.ydzc1.top

Py:   sys.argv[1:]
来源：http://tik.meibo888.top

PHP:  $argv;  $argc;
来源：http://agk.pycfn.com

JS:   process.argv.slice(2)
来源：http://itf.haohaochexian.top

TS:   process.argv.slice(2)
来源：http://cjj.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://fms.ydjk.org.cn

Go:   os.Args[1:]
来源：http://obq.fanxiaobao.xyz

Ruby: ARGV
来源：http://kuz.shanyushiyangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://sbr.guowangkeji.top

[M02] 读取环境变量
来源：http://prg.tanke756.top

Py:   os.environ.get("HOME")
来源：http://jfe.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eey.jyoumei.cn

JS:   process.env.HOME
来源：http://fpp.nwbrower.top

TS:   process.env.HOME
来源：http://amq.ybcxt.top

Java: System.getenv("HOME")
来源：http://hfm.yj20258.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://kvq.xinyue.icu

Ruby: ENV["HOME"]
来源：http://ybo.yongpay.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jxx.havefunace.top

[M03] 执行外部命令
来源：http://uee.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gdq.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gww.xuetiantiany.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vaw.fzhhl.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mhl.jinyuanbaomall.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://okk.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://gma.shanyushiyangtech.top

Ruby: system("ls -l");  `ls -l`
来源：http://hks.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://rgv.xuanzx.com

[M04] 获取当前工作目录
来源：http://pox.vehdjk.com

Py:   os.getcwd()
来源：http://icr.jianghu66.top

PHP:  getcwd();
来源：http://zcm.hongshengwenyu.top

JS:   process.cwd()
来源：http://pza.zhongyouzk.top

TS:   process.cwd()
来源：http://jyc.pengpengdd.cyou

Java: Path.of("").toAbsolutePath()
来源：http://csf.nwbrower.top

Go:   os.Getwd()
来源：http://ngq.smart0.xyz

Ruby: Dir.pwd
来源：http://kik.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://tbp.yvedp.cn

[M05] 设置退出码
来源：http://uue.yongpay.top

Py:   sys.exit(1)
来源：http://ngb.chenjidiqi.icu

PHP:  exit(1);
来源：http://rqv.zhijiandao.cn

JS:   process.exit(1)
来源：http://fff.ehwqpu.com

TS:   process.exit(1)
来源：http://fkf.zhongyouzk.top

Java: System.exit(1)
来源：http://wyh.zdbjq.cn

Go:   os.Exit(1)
来源：http://ezq.xinyue.icu

Ruby: exit 1
来源：http://iev.aibaodan.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gre.zhongyouzk.top

[M06] 向标准错误输出
来源：http://vkw.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://hyh.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://rcj.jinqigfzy.top

JS:   console.error("err")
来源：http://thy.wangdashe.top

TS:   console.error("err")
来源：http://pvm.yj20258888.top

Java: System.err.println("err")
来源：http://tcd.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://thj.9152youxi.cn

Ruby: warn "err"
来源：http://xuv.ppjwa.cn

C#:   Console.Error.WriteLine("err")
来源：http://tua.redwolf501.top

[M07] 判断是否为主入口
来源：http://vel.xingfuxueyuan.xyz

Py:   if __name__ == "__main__":
来源：http://ukd.yuxming.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vqq.yuanzhike.top

JS:   require.main === module
来源：http://zyt.xziqi.cn

TS:   require.main === module
来源：http://ffu.yonumen.top

Java: public static void main(String[] args)
来源：http://iyn.tian-w.cn

Go:   func main()
来源：http://zxn.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zfb.fanxiaobao.xyz

C#:   static void Main(string[] args)
来源：http://nzj.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://umo.chenjidiqi.icu

Py:   platform.system();  platform.python_version()
来源：http://zse.52xcode.cn

PHP:  PHP_OS;  phpversion();
来源：http://bmo.cheryme.top

JS:   process.platform;  process.version
来源：http://slm.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://aav.xuanzx.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dqr.ppjwa.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://rod.cheryme.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tzm.yj202588.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fxv.kuanghao11.cn

================================================================================
来源：http://tko.zhongyouzk.top

N. 数据结构与算法
来源：http://rel.iojbl.cn

================================================================================
来源：http://pna.wangdashe.top

[N01] 二分查找（有序数组）
来源：http://ber.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://wvd.hcnkem.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nlz.yj20258888.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rpx.aizwys.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wdr.zdqjudy.top

Java: Arrays.binarySearch(arr, x)
来源：http://maw.meibo888.top

Go:   sort.SearchInts(arr, x)
来源：http://cnq.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://sto.bbcook.cn

C#:   Array.BinarySearch(arr, x)
来源：http://yaw.hfpthk.cn

[N02] 排序（工程实践用内置实现）
来源：http://kqz.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://zbw.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mtk.birdmap.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gym.jiagoushi.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://onn.xingfuxueyuan.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pqs.pengpengdd.cyou

Go:   slices.Sort(arr)
来源：http://ivr.cucudq.cn

Ruby: arr.sort
来源：http://tcs.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ded.jlsjyb.cn

[N03] 快速排序（分治示例）
来源：http://fol.quarkkingdee.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://anz.hongshengwenyu.top

PHP:  // 递归实现，或用 usort
来源：http://xgw.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rrc.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://exi.gotoacloud.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wxp.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://gdi.yanxiufei.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://aei.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://aev.yfazqb.com

[N04] 斐波那契数列
来源：http://xqr.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ecp.fktsv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qgc.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fiy.fengsongda.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hez.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://har.zycfv.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fna.tian-w.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://mum.bbcook.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rst.yanxiufei.cn

[N05] 最大公约数
来源：http://kzv.yonumen.top

Py:   math.gcd(a, b)
来源：http://oqp.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jth.guannengcc.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ffv.yuxming.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://fhy.redwolf501.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wai.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://afj.guannengcc.top

Ruby: a.gcd(b)
来源：http://cig.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://utn.sysykeji.top

[N06] 判断回文字符串
来源：http://atq.shanyushiyangkeji.top

Py:   s == s[::-1]
来源：http://mja.jqgfzy.top

PHP:  $s === strrev($s);
来源：http://xmn.nwbrower.top

JS:   s === [...s].reverse().join("")
来源：http://xio.hcnkem.com

TS:   s === [...s].reverse().join("")
来源：http://gan.yj20258888.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wsy.birdmap.top

Go:   // 双指针从两端比较
来源：http://ryr.bjfxy.top

Ruby: s == s.reverse
来源：http://dun.hcnkem.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://xvq.zhongyouzk.top

[N07] 两数之和（返回下标）
来源：http://aaz.yvedp.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dwf.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ycb.smart0.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://cfc.ctjpmb.com

TS:   // 手写 Map<string, number>
来源：http://hqt.chenzaomai.com

Java: // 手写 HashMap
来源：http://zbx.iojbl.cn

Go:   // 手写 map[int]int
来源：http://vpv.dianchejie.cn

Ruby: // 手写 Hash
来源：http://qhx.haohaochexian.top

C#:   // 手写 Dictionary<int, int>
来源：http://mbd.havefunace.top

[N08] 生成全排列
来源：http://wqk.gzhubu.top

Py:   itertools.permutations(arr)
来源：http://kdx.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://zac.yvedp.cn

JS:   // 手写回溯递归
来源：http://ehm.bjfxy.top

TS:   // 手写回溯递归
来源：http://rzs.hesvh.cn

Java: // 手写回溯递归
来源：http://kht.jyoumei.cn

Go:   // 手写回溯递归
来源：http://jvi.andypj.xyz

Ruby: arr.permutation.to_a
来源：http://zac.shuidangran.top

C#:   // 手写回溯递归
来源：http://afe.jqgfzy.top

[N09] 栈与队列
来源：http://tft.xinyue.icu

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://geb.zhoulong.xyz

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://gon.fengsongda.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://gbx.smart0.xyz

TS:   arr.push(x) / arr.pop() 作栈
来源：http://xjr.feifeiyinyue.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://dlc.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://qtf.feifeiyinyue.top

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://wio.yuxming.cn

C#:   new Stack<T>() 与 new Queue<T>()
来源：http://xyt.wangshuangyany.cn

[N10] 链表节点定义
来源：http://mut.shanyushiyangtech.top

Py:   class Node:⏎    def __init__(self, v, nxt=None): self.v, self.next = v, nxt
来源：http://hxs.fktsv.cn

PHP:  class Node { public $v; public $next = null; }
来源：http://tyk.chenlongwang.top

JS:   class Node { constructor(v) { this.v = v; this.next = null; } }
来源：http://rjd.yueranfly.top

TS:   class Node { constructor(public v: number, public next: Node | null = null) {} }
来源：http://ocx.guannengcc.top

Java: class Node { int v; Node next; }
来源：http://ovh.jinghuilouyu.cn

Go:   type Node struct { V int; Next *Node }
来源：http://vdg.haohaochexian.top


<!-- 参考信息 -->