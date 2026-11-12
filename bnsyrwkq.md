代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xsa.hnxiangtu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://uee.fktsv.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://mxo.zhiwuduotai.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://dph.316326.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://kkd.fengsongda.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vdm.tarul.cn

[J09] 时区处理
来源：http://usu.birdmap.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qlg.xuetiantiany.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://zqu.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oeg.mhx1999.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lmq.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jwt.sxryk.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eay.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jxj.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://lid.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://ipk.ywan-chungtsiang.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ftl.cqqwz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gcm.hywenlv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oem.guowangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://drq.yuanzhike.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wmq.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gex.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wue.xuanzx.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://idi.jqgfzy.top

================================================================================
来源：http://bxw.quarkkingdee.top

K. JSON 与序列化
来源：http://gik.zhengqikj.top

================================================================================
来源：http://itt.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://exi.bbcook.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zri.yuanzhike.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://isx.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://lvz.nwbrower.top

TS:   JSON.stringify(obj)
来源：http://kdw.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tek.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://qlm.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://zfs.jiagoushi.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xiu.daria6918.cn

[K02] JSON 字符串转对象
来源：http://boy.hfpthk.cn

Py:   json.loads(s)
来源：http://vrk.tianlin.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uqa.zdbjq.cn

JS:   JSON.parse(s)
来源：http://wfc.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://uwk.ppjwa.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vcl.guannengcc.top

Go:   json.Unmarshal(data, &v)
来源：http://ejw.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://ztk.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mfc.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://hwy.pycfn.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://biz.pycfn.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dyi.cashguo.top

JS:   JSON.stringify(obj, null, 2)
来源：http://cbl.zhoulong.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://slc.zdqjudy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ciw.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xhp.jianghu66.top

Ruby: JSON.pretty_generate(obj)
来源：http://pox.zhaomingkeji.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pcl.aizwys.cn

[K04] 读取 JSON 文件
来源：http://ovs.yueranfly.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ljm.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vju.yfazqb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bdc.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gkv.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oyz.uphjek.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://iek.yueranfly.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://sfr.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ryx.hcnkem.com

[K05] 深拷贝对象
来源：http://fzb.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://eag.wangshuangyany.cn

PHP:  unserialize(serialize($obj));
来源：http://pvk.hywenlv.cn

JS:   structuredClone(obj)
来源：http://lse.c1oappe.top

TS:   structuredClone(obj)
来源：http://rvq.fzhhl.top

Java: // 手写拷贝构造，或序列化往返
来源：http://yym.yueranfly.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://evp.52xcode.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://smt.zhoulong.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://muc.hfpthk.cn

[K06] 解析 URL 查询串
来源：http://ogc.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lfc.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ujf.snrcjt.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://icj.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lgh.jinyuanbaomall.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lfy.zdbjq.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://fsg.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jee.shanyushiyangkeji.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zdc.cheryme.top

[K07] 进制转换
来源：http://fdq.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gyz.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://uws.tian-w.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ziq.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://opy.fehbvm.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pwp.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tut.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://pey.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://emk.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://xvn.havefunace.top

Py:   pickle.dumps(obj)
来源：http://wwe.daxiang520.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bxw.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://zck.zdqjudy.top

TS:   v8.serialize(obj)        // Node
来源：http://cja.feifeiyinyue.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kwm.gogol.net.cn

Go:   encoding/gob
来源：http://gbf.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://mlb.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://clx.zhengqikj.top

================================================================================
来源：http://vyf.quarkkingdee.top

L. 网络请求
来源：http://fww.svipenyu.cn

================================================================================
来源：http://hzq.zhixingplan.top

[L01] 发送 GET 请求
来源：http://jrw.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://slb.zhixingplan.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bed.fzhhl.top

JS:   await fetch(url)
来源：http://vjr.guowangkeji.top

TS:   await fetch(url)
来源：http://wrl.ivvv.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dxt.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://aij.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://vce.cashguo.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pck.yangfankeji.com

[L02] 发送 POST JSON
来源：http://vrf.xylfe.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tkq.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://udi.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dgl.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lbh.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jjg.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eoj.zdbjq.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gkh.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://oit.yj202588.top

[L03] 设置自定义请求头
来源：http://jpq.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://poa.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sxs.wangshuangyany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qlu.jqgfzy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://seb.jqgufenzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ljl.pycfn.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://onh.snrcjt.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zvp.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ggx.pycfn.com

[L04] 设置超时
来源：http://vca.jiagoushi.top

Py:   requests.get(url, timeout=5)
来源：http://pgz.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fxt.ywan-chungtsiang.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://aso.guowangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ekw.ppjwa.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wvy.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://rbe.ydjk.org.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tkw.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qbc.jianghu66.top

[L05] 上传文件（multipart）
来源：http://lcg.316326.xyz

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://voh.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zfm.xingfuxueyuan.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vwi.yuxming.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ppc.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tjv.jinghuilouyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fim.9152youxi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ive.gogol.net.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ovw.gzhubu.top

[L06] 解析响应为 JSON
来源：http://ian.yfazqb.com

Py:   resp.json()
来源：http://wod.pycfn.com

PHP:  json_decode($body, true);
来源：http://gtm.zhixingplan.top

JS:   await resp.json()
来源：http://lmo.hcnkem.com

TS:   await resp.json()
来源：http://aft.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://wxr.0kj1m.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mon.guannengcc.top

Ruby: JSON.parse(resp.body)
来源：http://rus.guannengcc.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lbv.svipenyu.cn

[L07] 处理 HTTP 状态码
来源：http://lec.cashguo.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zgh.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jsj.zhoulong.xyz

JS:   resp.ok;  resp.status
来源：http://wmx.xinyue.icu

TS:   resp.ok;  resp.status
来源：http://ntj.epnwcf.com

Java: resp.statusCode()
来源：http://aab.xziqi.cn

Go:   resp.StatusCode
来源：http://aeb.aizwys.cn

Ruby: resp.code.to_i
来源：http://kav.yonumen.top

C#:   (int)resp.StatusCode
来源：http://obs.bbcook.cn

[L08] 并发请求多个地址
来源：http://osz.tanke756.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://els.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://iyf.jqgufenzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://inc.andypj.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cam.nanxuanxn.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://wxm.wangdashe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tah.sxryk.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://chm.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bqa.yuxming.cn

================================================================================
来源：http://lou.kuanghao11.cn

M. 命令行 / 进程 / 环境
来源：http://fqq.gogol.net.cn

================================================================================
来源：http://tma.svipenyu.cn

[M01] 读取命令行参数
来源：http://ldw.ehwqpu.com

Py:   sys.argv[1:]
来源：http://vec.jinqigfzy.top

PHP:  $argv;  $argc;
来源：http://qgw.hnxiangtu.top

JS:   process.argv.slice(2)
来源：http://gxv.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://aah.0kj1m.cn

Java: args 数组（main 方法参数）
来源：http://hvv.zycfv.cn

Go:   os.Args[1:]
来源：http://psu.ehwqpu.com

Ruby: ARGV
来源：http://swe.dianchejie.cn

C#:   args 数组（Main 方法参数）
来源：http://qgs.jqgufenzy.top

[M02] 读取环境变量
来源：http://xnb.hywenlv.cn

Py:   os.environ.get("HOME")
来源：http://uek.fzhhl.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jyt.zhiwuduotai.top

JS:   process.env.HOME
来源：http://tib.zdbjq.cn

TS:   process.env.HOME
来源：http://uqa.ydjk.org.cn

Java: System.getenv("HOME")
来源：http://qjw.yueranfly.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qra.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://lxf.epnwcf.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://eac.tianlin.xyz

[M03] 执行外部命令
来源：http://lsq.jiagoushi.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ocz.gogol.net.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://frh.shzxlz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xtc.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://dim.redwolf501.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wnh.guannengcc.top

Go:   exec.Command("ls", "-l").Output()
来源：http://opn.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://crs.xuetiantiany.cn

C#:   Process.Start("ls", "-l");
来源：http://ejg.yangfankeji.com

[M04] 获取当前工作目录
来源：http://wro.jyoumei.cn

Py:   os.getcwd()
来源：http://tet.daxiang520.top

PHP:  getcwd();
来源：http://kyd.andypj.xyz

JS:   process.cwd()
来源：http://ukx.havefunace.top

TS:   process.cwd()
来源：http://qqd.jianghu66.top

Java: Path.of("").toAbsolutePath()
来源：http://dby.gaohongyu789.top

Go:   os.Getwd()
来源：http://xaq.vqdsnc.cn

Ruby: Dir.pwd
来源：http://gxc.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eof.yj20258.top

[M05] 设置退出码
来源：http://mrl.ivvv.top

Py:   sys.exit(1)
来源：http://hkr.sjlbkw.cn

PHP:  exit(1);
来源：http://quj.jinqigufen.top

JS:   process.exit(1)
来源：http://kms.fzhhl.top

TS:   process.exit(1)
来源：http://utm.ivvv.top

Java: System.exit(1)
来源：http://qqw.andypj.xyz

Go:   os.Exit(1)
来源：http://ucz.nanxinkj.top

Ruby: exit 1
来源：http://wqj.tianlin.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ajn.fktsv.cn

[M06] 向标准错误输出
来源：http://nsw.gaohongyu789.top

Py:   print("err", file=sys.stderr)
来源：http://ldd.pengpengdd.cyou

PHP:  fwrite(STDERR, "err\n");
来源：http://gsy.bbcook.cn

JS:   console.error("err")
来源：http://gyc.ivvv.top

TS:   console.error("err")
来源：http://ktt.dianchejie.cn

Java: System.err.println("err")
来源：http://bnh.zdbjq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://caw.tanke756.top

Ruby: warn "err"
来源：http://qvm.haohaochexian.top

C#:   Console.Error.WriteLine("err")
来源：http://lsm.haohaochexian.top

[M07] 判断是否为主入口
来源：http://eam.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://oqo.shangyingyoupin.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jti.tanke756.top

JS:   require.main === module
来源：http://buv.shangyingyoupin.top

TS:   require.main === module
来源：http://dle.yj20258888.top

Java: public static void main(String[] args)
来源：http://yyj.gzhubu.top

Go:   func main()
来源：http://gvr.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tiq.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://dcq.sysykeji.top

[M08] 获取系统与运行时信息
来源：http://rff.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://vqc.tarul.cn

PHP:  PHP_OS;  phpversion();
来源：http://wat.hysaishi.cn

JS:   process.platform;  process.version
来源：http://mle.nanxinkj.top

TS:   process.platform;  process.version
来源：http://avs.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://adt.zhijiandao.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://tlw.hammf.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nje.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kpz.zycfv.cn

================================================================================
来源：http://mvy.ywan-chungtsiang.top

N. 数据结构与算法
来源：http://hdx.shzxlz.cn

================================================================================
来源：http://mlf.bbcook.cn

[N01] 二分查找（有序数组）
来源：http://fmt.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://nvy.pycfn.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ctd.yj20258.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uat.fzhhl.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zmw.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://nhe.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://apo.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://wvi.ybcxt.top

C#:   Array.BinarySearch(arr, x)
来源：http://pye.zhoulong.xyz

[N02] 排序（工程实践用内置实现）
来源：http://rfe.chenzaomai.com

Py:   sorted(arr);  arr.sort()
来源：http://dbu.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://zyq.ivvv.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xrf.tarul.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lgs.hysaishi.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lka.hammf.cn

Go:   slices.Sort(arr)
来源：http://xgz.yj202588.top

Ruby: arr.sort
来源：http://yny.epnwcf.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://vek.uphjek.com

[N03] 快速排序（分治示例）
来源：http://bvi.cashguo.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://byf.yuanzhike.top

PHP:  // 递归实现，或用 usort
来源：http://jng.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kcr.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sdo.gogol.net.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rjv.aibaodan.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zwj.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bnw.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qxd.jyoumei.cn

[N04] 斐波那契数列
来源：http://qld.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://inr.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kgt.sweek.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hsh.zhoulong.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ola.shzxlz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://whs.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eev.316326.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://pym.jiagoushi.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pgn.daxiang520.top

[N05] 最大公约数
来源：http://hec.cheryme.top

Py:   math.gcd(a, b)
来源：http://xpj.nanxinkj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fvo.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jfu.sufxvd.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jdz.kuanghao11.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://oyx.sweek.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ksy.tianlin.xyz

Ruby: a.gcd(b)
来源：http://jhy.zdqjudy.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://khy.uphjek.com

[N06] 判断回文字符串
来源：http://rit.xziqi.cn

Py:   s == s[::-1]
来源：http://ylt.daxiang520.top

PHP:  $s === strrev($s);
来源：http://scp.yonumen.top


<!-- 参考信息 -->