代发 wailian999

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://nvs.jyoumei.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wts.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://swi.zhoulong.xyz

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cnc.daxiang520.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ujn.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://nwm.haohaochexian.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://vlf.quarkkingdee.top

[J10] 取今天 / 本月第一天
来源：http://awr.xingfuxueyuan.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://pxo.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://akq.hongshengwenyu.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://are.gzhubu.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://szd.sjlbkw.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xni.guannengcc.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ddh.zycfv.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gfx.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nyx.yj20258888.top

================================================================================
来源：http://vec.haohaochexian.top

K. JSON 与序列化
来源：http://fll.zhixingplan.top

================================================================================
来源：http://qwm.hysaishi.cn

[K01] 对象转 JSON 字符串
来源：http://akb.smart0.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qod.shangyingyoupin.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uvi.epnwcf.com

JS:   JSON.stringify(obj)
来源：http://hrt.yvedp.cn

TS:   JSON.stringify(obj)
来源：http://ahk.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://chm.zhiwuduotai.top

Go:   json.Marshal(obj)
来源：http://kgz.cheryme.top

Ruby: obj.to_json                                     // require "json"
来源：http://oaz.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jye.yuanzhike.top

[K02] JSON 字符串转对象
来源：http://xxd.snrcjt.cn

Py:   json.loads(s)
来源：http://kyg.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://omh.0kj1m.cn

JS:   JSON.parse(s)
来源：http://hat.ydzc1.top

TS:   JSON.parse(s)
来源：http://rey.quarkkingdee.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://fym.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://syq.sysykeji.top

Ruby: JSON.parse(s)
来源：http://wns.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qek.quarkkingdee.top

[K03] JSON 美化输出（带缩进）
来源：http://ndf.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ifp.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lsl.daria6918.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bgz.fanxiaobao.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ref.vehdjk.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gep.sxryk.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jxq.cashguo.top

Ruby: JSON.pretty_generate(obj)
来源：http://nrb.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sjy.xinyue.icu

[K04] 读取 JSON 文件
来源：http://pnn.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ocb.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mlz.xingfuxueyuan.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sbr.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://iro.fengsongda.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://szl.shuidangran.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wra.zdbjq.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://wkv.ybcxt.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qcs.gzhubu.top

[K05] 深拷贝对象
来源：http://qae.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://akl.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://chd.yueranfly.top

JS:   structuredClone(obj)
来源：http://knv.birdmap.top

TS:   structuredClone(obj)
来源：http://rvh.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ijz.ivvv.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gtv.jinqigfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://elw.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xoi.tanke756.top

[K06] 解析 URL 查询串
来源：http://nzr.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rgr.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://tjt.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://axr.ydjk.org.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://npr.smart0.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rur.snrcjt.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bvi.ydzc1.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://thx.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bqo.9152youxi.cn

[K07] 进制转换
来源：http://exy.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gum.zdqjudy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jnp.nanxuanxn.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://aak.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ygn.fengsongda.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pay.wangdashe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xfu.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://def.yuanzhike.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kve.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://lzj.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://rdj.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nrk.hongshengwenyu.top

JS:   v8.serialize(obj)        // Node
来源：http://txy.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://otm.jlsjyb.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ldb.shuidangran.top

Go:   encoding/gob
来源：http://oou.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://ngk.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jqc.redwolf501.top

================================================================================
来源：http://pxt.yfazqb.com

L. 网络请求
来源：http://fvx.c1oappe.top

================================================================================
来源：http://gkh.cucudq.cn

[L01] 发送 GET 请求
来源：http://mbh.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mai.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wkw.ybcxt.top

JS:   await fetch(url)
来源：http://akv.zhongyouzk.top

TS:   await fetch(url)
来源：http://ykz.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ptc.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://ejf.cheryme.top

Ruby: Net::HTTP.get(URI(url))
来源：http://gkt.jlsjyb.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jam.shzxlz.cn

[L02] 发送 POST JSON
来源：http://avh.fktsv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bkq.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://xuh.mhx1999.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yoc.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wgu.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vhf.quarkkingdee.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fnb.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://eep.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bwj.ydzc1.top

[L03] 设置自定义请求头
来源：http://qip.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xia.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yhh.shanyushiyangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nyj.aizwys.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jzh.zycfv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://aha.ctjpmb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vsb.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ibz.shangyingyoupin.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jpm.hcnkem.com

[L04] 设置超时
来源：http://adj.ehwqpu.com

Py:   requests.get(url, timeout=5)
来源：http://qmq.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ovu.yj20258.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cdu.redwolf501.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xgm.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tyu.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://sue.aizwys.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://phz.316326.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ebe.guowangkeji.top

[L05] 上传文件（multipart）
来源：http://wgz.yfazqb.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://pow.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gtk.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tkq.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kiu.ydjk.org.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://woh.aibaodan.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xng.gogol.net.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tcn.daxiang520.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jbp.chenjidiqi.icu

[L06] 解析响应为 JSON
来源：http://law.yonumen.top

Py:   resp.json()
来源：http://ruq.yuanzhike.top

PHP:  json_decode($body, true);
来源：http://ajq.ctjpmb.com

JS:   await resp.json()
来源：http://dey.uphjek.com

TS:   await resp.json()
来源：http://qfd.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://evk.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ygx.xylfe.cn

Ruby: JSON.parse(resp.body)
来源：http://gqx.yj20258888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pvc.iojbl.cn

[L07] 处理 HTTP 状态码
来源：http://wza.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://coj.yj20258.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sul.tarul.cn

JS:   resp.ok;  resp.status
来源：http://pku.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://avd.9152youxi.cn

Java: resp.statusCode()
来源：http://isc.epnwcf.com

Go:   resp.StatusCode
来源：http://ewx.yj20258.top

Ruby: resp.code.to_i
来源：http://rdo.feifeiyinyue.top

C#:   (int)resp.StatusCode
来源：http://lrt.yongpay.top

[L08] 并发请求多个地址
来源：http://jmb.guowangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jpa.fehbvm.com

PHP:  curl_multi_init() 系列
来源：http://cbe.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nri.yj20258.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yci.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mmq.yuanzhike.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gfs.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://exi.9152youxi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ync.jiagoushi.top

================================================================================
来源：http://jdk.jyoumei.cn

M. 命令行 / 进程 / 环境
来源：http://iti.yvedp.cn

================================================================================
来源：http://srn.yj202588.top

[M01] 读取命令行参数
来源：http://laa.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://nsn.smart0.xyz

PHP:  $argv;  $argc;
来源：http://ymi.iojbl.cn

JS:   process.argv.slice(2)
来源：http://udc.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://fwa.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://ejw.smart0.xyz

Go:   os.Args[1:]
来源：http://eaf.sysykeji.top

Ruby: ARGV
来源：http://ica.tanke756.top

C#:   args 数组（Main 方法参数）
来源：http://nwh.iojbl.cn

[M02] 读取环境变量
来源：http://who.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://suz.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://czj.sjlbkw.cn

JS:   process.env.HOME
来源：http://sto.ywan-chungtsiang.top

TS:   process.env.HOME
来源：http://ykf.zhijiandao.cn

Java: System.getenv("HOME")
来源：http://ads.c1oappe.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xzg.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://fum.yongpay.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pwk.ctjpmb.com

[M03] 执行外部命令
来源：http://ycw.ctjpmb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kay.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qcj.svipenyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kpm.zycfv.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://pbo.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ppc.sufxvd.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://vak.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://dlq.tarul.cn

C#:   Process.Start("ls", "-l");
来源：http://hag.chenjidiqi.icu

[M04] 获取当前工作目录
来源：http://gbq.bbcook.cn

Py:   os.getcwd()
来源：http://mqb.xziqi.cn

PHP:  getcwd();
来源：http://evb.shangyingyoupin.top

JS:   process.cwd()
来源：http://ogv.cqqwz.cn

TS:   process.cwd()
来源：http://wbb.daxiang520.top

Java: Path.of("").toAbsolutePath()
来源：http://syd.zhaomingkeji.xyz

Go:   os.Getwd()
来源：http://kbv.redwolf501.top

Ruby: Dir.pwd
来源：http://itc.zhoulong.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://wcl.svipenyu.cn

[M05] 设置退出码
来源：http://rmg.hywenlv.cn

Py:   sys.exit(1)
来源：http://tju.c1oappe.top

PHP:  exit(1);
来源：http://fqg.hcnkem.com

JS:   process.exit(1)
来源：http://gts.yvedp.cn

TS:   process.exit(1)
来源：http://inr.aibaodan.cn

Java: System.exit(1)
来源：http://yzz.zhongyouzk.top

Go:   os.Exit(1)
来源：http://hfv.feifeiyinyue.top

Ruby: exit 1
来源：http://avh.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kio.yj202588.top

[M06] 向标准错误输出
来源：http://kvg.jiagoushi.top

Py:   print("err", file=sys.stderr)
来源：http://oje.yj20258.top

PHP:  fwrite(STDERR, "err\n");
来源：http://tzi.zdqjudy.top

JS:   console.error("err")
来源：http://tcr.xziqi.cn

TS:   console.error("err")
来源：http://gog.zhoulong.xyz

Java: System.err.println("err")
来源：http://nlp.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ccv.daria6918.cn

Ruby: warn "err"
来源：http://qgu.cdnleiting.top

C#:   Console.Error.WriteLine("err")
来源：http://vpp.shuidangran.top

[M07] 判断是否为主入口
来源：http://wxb.mhx1999.top

Py:   if __name__ == "__main__":
来源：http://pba.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vwu.yj202588.top

JS:   require.main === module
来源：http://xaz.ywan-chungtsiang.top

TS:   require.main === module
来源：http://ajt.yj20258888.top

Java: public static void main(String[] args)
来源：http://lbp.yangfankeji.com

Go:   func main()
来源：http://mtb.hongshengwenyu.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://pni.cucudq.cn

C#:   static void Main(string[] args)
来源：http://rnm.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://smx.zycfv.cn

Py:   platform.system();  platform.python_version()
来源：http://vrn.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://mie.guowangkeji.top

JS:   process.platform;  process.version
来源：http://muk.sufxvd.cn

TS:   process.platform;  process.version
来源：http://iyy.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ply.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bdu.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://auy.hcnkem.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://ejo.hnxiangtu.top

================================================================================
来源：http://lxo.sysykeji.top

N. 数据结构与算法
来源：http://lki.guowangkeji.top

================================================================================
来源：http://ppo.yfazqb.com

[N01] 二分查找（有序数组）
来源：http://fnb.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://hia.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://eov.ydjk.org.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nrn.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ego.shuidangran.top

Java: Arrays.binarySearch(arr, x)
来源：http://btk.chenzaomai.com

Go:   sort.SearchInts(arr, x)
来源：http://zxi.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://dmm.jinqigfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://sfq.yueranfly.top

[N02] 排序（工程实践用内置实现）
来源：http://bal.svipenyu.cn

Py:   sorted(arr);  arr.sort()
来源：http://odb.fktsv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hgd.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://rmx.yj20258.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cpg.ivvv.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://esj.ehwqpu.com

Go:   slices.Sort(arr)
来源：http://psz.smart0.xyz

Ruby: arr.sort
来源：http://bgj.yj202588.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://mmw.jqgfzy.top

[N03] 快速排序（分治示例）
来源：http://vne.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sxq.meibo888.top

PHP:  // 递归实现，或用 usort
来源：http://xuw.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fkj.hesvh.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hxs.gaohongyu789.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rdu.zhongyouzk.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://iuv.daria6918.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://axj.zycfv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hpt.fengsongda.top

[N04] 斐波那契数列
来源：http://tfb.kuanghao11.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hms.yfazqb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://zhd.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bgt.gogol.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://otm.jqgufenzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://jhv.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mvi.yangfankeji.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://xhn.zdbjq.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mvy.nanxinkj.top

[N05] 最大公约数
来源：http://nkj.sxryk.cn

Py:   math.gcd(a, b)
来源：http://hfj.cashguo.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fzw.yuanzhike.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://brl.jinyuanbaomall.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://chx.hammf.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oao.sjlbkw.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://vkr.ybcxt.top

Ruby: a.gcd(b)
来源：http://jol.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bxp.nanxinkj.top

[N06] 判断回文字符串
来源：http://kzt.sjlbkw.cn

Py:   s == s[::-1]
来源：http://cts.haohaochexian.top

PHP:  $s === strrev($s);
来源：http://xbh.yfazqb.com

JS:   s === [...s].reverse().join("")
来源：http://qok.meibo888.top

TS:   s === [...s].reverse().join("")
来源：http://wjx.sxryk.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zla.yangfankeji.com

Go:   // 双指针从两端比较
来源：http://hqg.haohaochexian.top

Ruby: s == s.reverse
来源：http://hhg.tian-w.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://nly.iojbl.cn

[N07] 两数之和（返回下标）
来源：http://wqq.c1oappe.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wjs.sxryk.cn


<!-- 参考信息 -->