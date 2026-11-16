代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xbq.meibo888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://heq.jinghuilouyu.cn

[J09] 时区处理
来源：http://mtq.kuanghao11.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://psp.jinyuanbaomall.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ivt.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jdn.bbcook.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://abh.gotoacloud.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gyu.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://vjo.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xcx.smart0.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://miu.aibaodan.cn

[J10] 取今天 / 本月第一天
来源：http://qtw.yvedp.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bif.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://wni.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://war.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://epl.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gra.xylfe.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://njv.jyoumei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ebv.bbcook.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bgf.zhongyouzk.top

================================================================================
来源：http://cxf.jinyuanbaomall.cn

K. JSON 与序列化
来源：http://gyw.haohaochexian.top

================================================================================
来源：http://zxc.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://teb.dashuyun.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ora.nanxinkj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gia.guowangkeji.top

JS:   JSON.stringify(obj)
来源：http://jmf.yj20258.top

TS:   JSON.stringify(obj)
来源：http://fwk.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://doz.nwbrower.top

Go:   json.Marshal(obj)
来源：http://cdw.zdqjudy.top

Ruby: obj.to_json                                     // require "json"
来源：http://mls.sxryk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://opg.zycfv.cn

[K02] JSON 字符串转对象
来源：http://arp.yj202588.top

Py:   json.loads(s)
来源：http://gan.aizwys.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cmi.jiagoushi.top

JS:   JSON.parse(s)
来源：http://ugo.gotoacloud.top

TS:   JSON.parse(s)
来源：http://bzg.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nee.shzxlz.cn

Go:   json.Unmarshal(data, &v)
来源：http://aim.zhoulong.xyz

Ruby: JSON.parse(s)
来源：http://fvt.yj202588.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://opm.52xcode.cn

[K03] JSON 美化输出（带缩进）
来源：http://lae.haohaochexian.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bbh.uphjek.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://imq.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fsb.dashuyun.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://gon.uphjek.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nwk.sufxvd.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://shh.jiagoushi.top

Ruby: JSON.pretty_generate(obj)
来源：http://hek.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dhg.ybcxt.top

[K04] 读取 JSON 文件
来源：http://vis.jqgufenzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://bvw.hywenlv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://tqx.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://irv.xingfuxueyuan.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mqx.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://llx.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vyo.zhiwuduotai.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://szc.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://enj.daxiang520.top

[K05] 深拷贝对象
来源：http://sud.jqgufenzy.top

Py:   copy.deepcopy(obj)
来源：http://mxx.dashuyun.cn

PHP:  unserialize(serialize($obj));
来源：http://mkt.hcnkem.com

JS:   structuredClone(obj)
来源：http://raa.zhaomingkeji.xyz

TS:   structuredClone(obj)
来源：http://nvq.meibo888.top

Java: // 手写拷贝构造，或序列化往返
来源：http://xyc.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ddd.gogol.net.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jdh.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://vrc.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://gsx.pengpengdd.cyou

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rtv.hnxiangtu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://okl.yuanzhike.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://skf.shanyushiyangkeji.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nmd.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wpa.shanyushiyangkeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ngp.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jwl.cdnleiting.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kid.xingfuxueyuan.xyz

[K07] 进制转换
来源：http://ugn.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://xbu.uphjek.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://dzr.nanxinkj.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://sef.zdbjq.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xpu.yuxming.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vfx.jyoumei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gag.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cue.hcnkem.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://quk.yj20258.top

[K08] 二进制序列化（非 JSON）
来源：http://nrm.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://eod.fehbvm.com

PHP:  serialize($obj);  unserialize($s);
来源：http://eqs.52xcode.cn

JS:   v8.serialize(obj)        // Node
来源：http://dyv.jqgfzy.top

TS:   v8.serialize(obj)        // Node
来源：http://imk.guowangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://klh.ybcxt.top

Go:   encoding/gob
来源：http://bre.haohaochexian.top

Ruby: Marshal.dump(obj)
来源：http://rjy.sweek.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lud.shzxlz.cn

================================================================================
来源：http://nld.hammf.cn

L. 网络请求
来源：http://ytt.yuxming.cn

================================================================================
来源：http://crk.jinqigufen.top

[L01] 发送 GET 请求
来源：http://nah.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zmg.jiagoushi.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://srg.wangshuangyany.cn

JS:   await fetch(url)
来源：http://gbe.xziqi.cn

TS:   await fetch(url)
来源：http://dor.epnwcf.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tiw.mhx1999.top

Go:   resp, err := http.Get(url)
来源：http://ved.shuidangran.top

Ruby: Net::HTTP.get(URI(url))
来源：http://vmj.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ulh.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://ijn.dashuyun.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oqk.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yiq.yanxiufei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ofz.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://umd.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wug.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://elt.nanxuanxn.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uzj.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pgu.wangshuangyany.cn

[L03] 设置自定义请求头
来源：http://vpm.pengpengdd.cyou

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yiq.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://wta.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nek.zdbjq.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zin.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tfd.aibaodan.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gyx.tian-w.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vwr.hongshengwenyu.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pwq.jyoumei.cn

[L04] 设置超时
来源：http://kwq.guannengcc.top

Py:   requests.get(url, timeout=5)
来源：http://gvt.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hmo.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wuq.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cfv.fktsv.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jse.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://iig.guowangkeji.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dlx.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://nwt.xylfe.cn

[L05] 上传文件（multipart）
来源：http://vcy.yuxming.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wzi.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uon.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wbj.shanyushiyangtech.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yfg.jinqigfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dfb.0kj1m.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://khf.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vlh.ppjwa.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wok.yonumen.top

[L06] 解析响应为 JSON
来源：http://eba.yj20258.top

Py:   resp.json()
来源：http://ubr.hammf.cn

PHP:  json_decode($body, true);
来源：http://jxp.yueranfly.top

JS:   await resp.json()
来源：http://ifs.sufxvd.cn

TS:   await resp.json()
来源：http://cwv.xuanzx.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ppo.ywan-chungtsiang.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wxz.0kj1m.cn

Ruby: JSON.parse(resp.body)
来源：http://qks.shzxlz.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vqj.jinghuilouyu.cn

[L07] 处理 HTTP 状态码
来源：http://ris.zdqjudy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oxl.bjfxy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jzf.c1oappe.top

JS:   resp.ok;  resp.status
来源：http://lbv.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://uyl.jyoumei.cn

Java: resp.statusCode()
来源：http://kzu.wangdashe.top

Go:   resp.StatusCode
来源：http://lqz.nwbrower.top

Ruby: resp.code.to_i
来源：http://hsu.ehwqpu.com

C#:   (int)resp.StatusCode
来源：http://uxv.shanyushiyangtech.top

[L08] 并发请求多个地址
来源：http://mrn.chenzaomai.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fdf.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://ndr.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bho.sysykeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rzf.iojbl.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://krv.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hvl.hongshengwenyu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dhi.yongpay.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kir.ydjk.org.cn

================================================================================
来源：http://srq.smart0.xyz

M. 命令行 / 进程 / 环境
来源：http://iob.hnxiangtu.top

================================================================================
来源：http://bbx.yueranfly.top

[M01] 读取命令行参数
来源：http://bin.yongpay.top

Py:   sys.argv[1:]
来源：http://oim.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://toz.tian-w.cn

JS:   process.argv.slice(2)
来源：http://inp.jinqigufen.top

TS:   process.argv.slice(2)
来源：http://zbq.xingfuxueyuan.xyz

Java: args 数组（main 方法参数）
来源：http://iez.fengsongda.top

Go:   os.Args[1:]
来源：http://uix.bjfxy.top

Ruby: ARGV
来源：http://qtj.xuanzx.com

C#:   args 数组（Main 方法参数）
来源：http://hgm.nanxinkj.top

[M02] 读取环境变量
来源：http://mww.yonumen.top

Py:   os.environ.get("HOME")
来源：http://srq.hnqzz.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://efn.ywan-chungtsiang.top

JS:   process.env.HOME
来源：http://ftx.feifeiyinyue.top

TS:   process.env.HOME
来源：http://juj.chenlongwang.top

Java: System.getenv("HOME")
来源：http://hvk.hesvh.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xhp.svipenyu.cn

Ruby: ENV["HOME"]
来源：http://itn.zhongyouzk.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dxd.jyoumei.cn

[M03] 执行外部命令
来源：http://ipc.tian-w.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dzf.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://snt.fehbvm.com

JS:   child_process.execSync("ls -l").toString()
来源：http://kcx.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://gre.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://psm.jqgufenzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://sru.uphjek.com

Ruby: system("ls -l");  `ls -l`
来源：http://kir.sjlbkw.cn

C#:   Process.Start("ls", "-l");
来源：http://aiw.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://ilg.yongpay.top

Py:   os.getcwd()
来源：http://noj.iojbl.cn

PHP:  getcwd();
来源：http://imb.yangfankeji.com

JS:   process.cwd()
来源：http://gsf.zycfv.cn

TS:   process.cwd()
来源：http://jzh.yj20258.top

Java: Path.of("").toAbsolutePath()
来源：http://vyq.iojbl.cn

Go:   os.Getwd()
来源：http://qdr.ivvv.top

Ruby: Dir.pwd
来源：http://qsx.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://wsq.jiagoushi.top

[M05] 设置退出码
来源：http://pnn.cqqwz.cn

Py:   sys.exit(1)
来源：http://rif.0kj1m.cn

PHP:  exit(1);
来源：http://qqj.bjfxy.top

JS:   process.exit(1)
来源：http://bbc.hysaishi.cn

TS:   process.exit(1)
来源：http://nww.hywenlv.cn

Java: System.exit(1)
来源：http://jfx.gzhubu.top

Go:   os.Exit(1)
来源：http://mwi.smart0.xyz

Ruby: exit 1
来源：http://jne.xziqi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pqs.dianchejie.cn

[M06] 向标准错误输出
来源：http://gxc.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://yvm.ctjpmb.com

PHP:  fwrite(STDERR, "err\n");
来源：http://bqx.cheryme.top

JS:   console.error("err")
来源：http://nqv.vehdjk.com

TS:   console.error("err")
来源：http://bnt.andypj.xyz

Java: System.err.println("err")
来源：http://wgz.vqdsnc.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rel.jinghuilouyu.cn

Ruby: warn "err"
来源：http://cub.fktsv.cn

C#:   Console.Error.WriteLine("err")
来源：http://udi.cqqwz.cn

[M07] 判断是否为主入口
来源：http://lsl.ivvv.top

Py:   if __name__ == "__main__":
来源：http://nge.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://aax.yj202588.top

JS:   require.main === module
来源：http://ssp.ywan-chungtsiang.top

TS:   require.main === module
来源：http://vtc.daxiang520.top

Java: public static void main(String[] args)
来源：http://veu.yuanzhike.top

Go:   func main()
来源：http://sha.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://cys.xingfuxueyuan.xyz

C#:   static void Main(string[] args)
来源：http://vjj.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://got.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://faq.yuanzhike.top

PHP:  PHP_OS;  phpversion();
来源：http://edg.yfazqb.com

JS:   process.platform;  process.version
来源：http://ncv.zdqjudy.top

TS:   process.platform;  process.version
来源：http://ftr.ydjk.org.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dqr.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ryz.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ofo.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kwr.birdmap.top

================================================================================
来源：http://kij.guannengcc.top

N. 数据结构与算法
来源：http://xhl.daxiang520.top

================================================================================
来源：http://bwk.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://wsr.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jjx.fktsv.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aow.guowangkeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zig.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nra.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://pqy.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://yrc.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://fqf.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://kxi.smart0.xyz

[N02] 排序（工程实践用内置实现）
来源：http://njb.xinyue.icu

Py:   sorted(arr);  arr.sort()
来源：http://ten.daria6918.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vro.ppjwa.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ldb.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://nsn.yvedp.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://mvm.guannengcc.top

Go:   slices.Sort(arr)
来源：http://ckw.nanxuanxn.top

Ruby: arr.sort
来源：http://ffh.dianchejie.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://btm.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://sjf.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jpa.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://var.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fog.havefunace.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://awy.hammf.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dak.hywenlv.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://jfg.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wvi.wangshuangyany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vzv.jinghuilouyu.cn

[N04] 斐波那契数列
来源：http://euy.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://cfk.tarul.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://yeo.cucudq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wtf.bbcook.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qjc.iojbl.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xcf.xuanzx.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://diq.aibaodan.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tcr.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://rbh.aibaodan.cn

[N05] 最大公约数
来源：http://dep.gzhubu.top

Py:   math.gcd(a, b)
来源：http://wlr.bjfxy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://adw.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://adu.jinghuilouyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vhj.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://bju.zhaomingkeji.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ail.fanxiaobao.xyz

Ruby: a.gcd(b)
来源：http://erj.aibaodan.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://rrr.daxiang520.top

[N06] 判断回文字符串
来源：http://dbx.quarkkingdee.top

Py:   s == s[::-1]
来源：http://pwg.zdbjq.cn

PHP:  $s === strrev($s);
来源：http://xrb.cashguo.top

JS:   s === [...s].reverse().join("")
来源：http://fxp.hywenlv.cn

TS:   s === [...s].reverse().join("")
来源：http://omf.tian-w.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ibd.316326.xyz

Go:   // 双指针从两端比较
来源：http://ivp.guannengcc.top


<!-- 参考信息 -->