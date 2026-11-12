代发 wailian999

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kka.fehbvm.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gcp.mhx1999.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ejw.hfpthk.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://kul.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://stu.gaohongyu789.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wvv.0kj1m.cn

[J09] 时区处理
来源：http://qzx.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://aex.hesvh.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bip.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jeg.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://cpw.ctjpmb.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://jwx.jinyuanbaomall.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yop.gotoacloud.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uhw.gotoacloud.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://atl.yueranfly.top

[J10] 取今天 / 本月第一天
来源：http://lfs.ivvv.top

Py:   date.today();  date.today().replace(day=1)
来源：http://dgm.yj202588.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://kdh.jinqigufen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://glk.jianghu66.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://dwv.jlsjyb.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jwl.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ldk.zhixingplan.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pfq.daria6918.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ltk.jinqigufen.top

================================================================================
来源：http://vhb.jinqigufen.top

K. JSON 与序列化
来源：http://pgc.mhx1999.top

================================================================================
来源：http://cjn.xziqi.cn

[K01] 对象转 JSON 字符串
来源：http://szp.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://byy.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jkb.bbcook.cn

JS:   JSON.stringify(obj)
来源：http://edq.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://phs.epnwcf.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kiu.hesvh.cn

Go:   json.Marshal(obj)
来源：http://rei.tarul.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hju.shzxlz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tsq.zhengqikj.top

[K02] JSON 字符串转对象
来源：http://jph.nwbrower.top

Py:   json.loads(s)
来源：http://scy.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xhl.vehdjk.com

JS:   JSON.parse(s)
来源：http://olo.jlsjyb.cn

TS:   JSON.parse(s)
来源：http://cge.hesvh.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pet.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://cdh.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://ouw.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zat.hfpthk.cn

[K03] JSON 美化输出（带缩进）
来源：http://ipn.fehbvm.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://mby.jianghu66.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kdi.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fsw.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://cva.gzhubu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://gxc.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vnx.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://mht.aizwys.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://phr.nwbrower.top

[K04] 读取 JSON 文件
来源：http://ave.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vul.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jvb.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oae.zhaomingkeji.xyz

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eim.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yzz.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tdx.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://gxt.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lln.yj20258888.top

[K05] 深拷贝对象
来源：http://keq.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://qbt.yuxming.cn

PHP:  unserialize(serialize($obj));
来源：http://tik.ctjpmb.com

JS:   structuredClone(obj)
来源：http://nhd.smart0.xyz

TS:   structuredClone(obj)
来源：http://vnj.yvedp.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vht.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ykj.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xfo.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://vxi.fktsv.cn

[K06] 解析 URL 查询串
来源：http://nsx.fehbvm.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bch.havefunace.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zaj.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yzn.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gqp.vqdsnc.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qgo.yuxming.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://kpm.jinghuilouyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lov.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zim.guowangkeji.top

[K07] 进制转换
来源：http://pqb.zhoulong.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://aiu.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ree.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bot.yongpay.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lsg.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qlo.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lup.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ggy.cdnleiting.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://sid.hnqzz.top

[K08] 二进制序列化（非 JSON）
来源：http://qaa.mhx1999.top

Py:   pickle.dumps(obj)
来源：http://xtz.shuidangran.top

PHP:  serialize($obj);  unserialize($s);
来源：http://odo.chenjidiqi.icu

JS:   v8.serialize(obj)        // Node
来源：http://hbi.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://xmd.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rdj.yj20258.top

Go:   encoding/gob
来源：http://tvi.sysykeji.top

Ruby: Marshal.dump(obj)
来源：http://lbh.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jwk.chenzaomai.com

================================================================================
来源：http://say.zhiwuduotai.top

L. 网络请求
来源：http://sqk.daria6918.cn

================================================================================
来源：http://iyr.gaohongyu789.top

[L01] 发送 GET 请求
来源：http://qka.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mpx.c1oappe.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cds.zdbjq.cn

JS:   await fetch(url)
来源：http://oue.quarkkingdee.top

TS:   await fetch(url)
来源：http://nok.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uap.ivvv.top

Go:   resp, err := http.Get(url)
来源：http://boq.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tur.xuanzx.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qym.nanxinkj.top

[L02] 发送 POST JSON
来源：http://udn.tarul.cn

Py:   requests.post(url, json={"a": 1})
来源：http://yxg.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wmi.sxryk.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ewz.uphjek.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mmb.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://frp.epnwcf.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sur.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://viu.cdnleiting.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lvk.yvedp.cn

[L03] 设置自定义请求头
来源：http://ryx.bbcook.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://czj.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gok.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cmj.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oos.xuetiantiany.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jie.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://eeu.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://khv.bjfxy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://pvs.andypj.xyz

[L04] 设置超时
来源：http://lkl.ybcxt.top

Py:   requests.get(url, timeout=5)
来源：http://xbb.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xey.hnqzz.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jye.ctjpmb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nok.ywan-chungtsiang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ejh.meibo888.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zgx.cucudq.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cag.shangyingyoupin.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tsv.iojbl.cn

[L05] 上传文件（multipart）
来源：http://lvd.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gra.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ohn.cqqwz.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jbf.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zjo.shangyingyoupin.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vir.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ver.wangdashe.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wlt.zhengqikj.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://npk.feifeiyinyue.top

[L06] 解析响应为 JSON
来源：http://zui.jinqigfzy.top

Py:   resp.json()
来源：http://bmo.redwolf501.top

PHP:  json_decode($body, true);
来源：http://tcb.xuanzx.com

JS:   await resp.json()
来源：http://ajq.52xcode.cn

TS:   await resp.json()
来源：http://dob.hongshengwenyu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://szn.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gcs.yanxiufei.cn

Ruby: JSON.parse(resp.body)
来源：http://tdl.tarul.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://haa.yonumen.top

[L07] 处理 HTTP 状态码
来源：http://ohz.mhx1999.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://avp.jyoumei.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://svj.xuetiantiany.cn

JS:   resp.ok;  resp.status
来源：http://kqd.tanke756.top

TS:   resp.ok;  resp.status
来源：http://rqx.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://obt.shuidangran.top

Go:   resp.StatusCode
来源：http://fns.fehbvm.com

Ruby: resp.code.to_i
来源：http://sai.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://ufw.52xcode.cn

[L08] 并发请求多个地址
来源：http://kmu.iojbl.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://xev.zhixingplan.top

PHP:  curl_multi_init() 系列
来源：http://odb.svipenyu.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jqt.dianchejie.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://etb.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nxv.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://hsw.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ggm.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oib.wangshuangyany.cn

================================================================================
来源：http://mrz.jqgfzy.top

M. 命令行 / 进程 / 环境
来源：http://qzk.andypj.xyz

================================================================================
来源：http://idl.jlsjyb.cn

[M01] 读取命令行参数
来源：http://ygx.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://rpz.jqgfzy.top

PHP:  $argv;  $argc;
来源：http://cff.jinqigfzy.top

JS:   process.argv.slice(2)
来源：http://qis.daria6918.cn

TS:   process.argv.slice(2)
来源：http://nua.jqgfzy.top

Java: args 数组（main 方法参数）
来源：http://zxp.iojbl.cn

Go:   os.Args[1:]
来源：http://flf.shuidangran.top

Ruby: ARGV
来源：http://qcg.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://gth.uphjek.com

[M02] 读取环境变量
来源：http://ltt.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://nmt.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fgi.hesvh.cn

JS:   process.env.HOME
来源：http://qyg.daxiang520.top

TS:   process.env.HOME
来源：http://wlx.svipenyu.cn

Java: System.getenv("HOME")
来源：http://vdm.zhixingplan.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xii.ppjwa.cn

Ruby: ENV["HOME"]
来源：http://qur.shangyingyoupin.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dzg.haohaochexian.top

[M03] 执行外部命令
来源：http://gru.c1oappe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fhe.zdbjq.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jlv.yvedp.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ros.jqgufenzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dwx.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ywu.hysaishi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bxp.52xcode.cn

Ruby: system("ls -l");  `ls -l`
来源：http://emf.tanke756.top

C#:   Process.Start("ls", "-l");
来源：http://rcb.yuanzhike.top

[M04] 获取当前工作目录
来源：http://ltv.tanke756.top

Py:   os.getcwd()
来源：http://wnr.aibaodan.cn

PHP:  getcwd();
来源：http://sug.jianghu66.top

JS:   process.cwd()
来源：http://fyj.hywenlv.cn

TS:   process.cwd()
来源：http://ezg.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://hjm.chenzaomai.com

Go:   os.Getwd()
来源：http://ogi.zhoulong.xyz

Ruby: Dir.pwd
来源：http://mvn.wangdashe.top

C#:   Directory.GetCurrentDirectory()
来源：http://lnz.birdmap.top

[M05] 设置退出码
来源：http://suy.gotoacloud.top

Py:   sys.exit(1)
来源：http://ydc.yj20258.top

PHP:  exit(1);
来源：http://gga.zdqjudy.top

JS:   process.exit(1)
来源：http://wwb.sweek.top

TS:   process.exit(1)
来源：http://aqu.xinyue.icu

Java: System.exit(1)
来源：http://rcv.tanke756.top

Go:   os.Exit(1)
来源：http://ymy.pycfn.com

Ruby: exit 1
来源：http://jrn.guowangkeji.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dni.quarkkingdee.top

[M06] 向标准错误输出
来源：http://tvl.sweek.top

Py:   print("err", file=sys.stderr)
来源：http://gqa.nanxinkj.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vrv.yuxming.cn

JS:   console.error("err")
来源：http://xki.svipenyu.cn

TS:   console.error("err")
来源：http://ahg.bbcook.cn

Java: System.err.println("err")
来源：http://cyh.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dew.shanyushiyangtech.top

Ruby: warn "err"
来源：http://gne.havefunace.top

C#:   Console.Error.WriteLine("err")
来源：http://ydg.xuetiantiany.cn

[M07] 判断是否为主入口
来源：http://zga.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://ifa.ehwqpu.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hra.yj20258.top

JS:   require.main === module
来源：http://ccx.hongshengwenyu.top

TS:   require.main === module
来源：http://zgl.fzhhl.top

Java: public static void main(String[] args)
来源：http://rcp.daria6918.cn

Go:   func main()
来源：http://ijc.gotoacloud.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tsc.hcnkem.com

C#:   static void Main(string[] args)
来源：http://kzz.316326.xyz

[M08] 获取系统与运行时信息
来源：http://ziz.redwolf501.top

Py:   platform.system();  platform.python_version()
来源：http://ixs.hammf.cn

PHP:  PHP_OS;  phpversion();
来源：http://syi.jinyuanbaomall.cn

JS:   process.platform;  process.version
来源：http://ahp.zycfv.cn

TS:   process.platform;  process.version
来源：http://cos.bjfxy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ejk.vehdjk.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://wal.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zaf.bjfxy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://rxh.shanyushiyangtech.top

================================================================================
来源：http://dlv.52xcode.cn

N. 数据结构与算法
来源：http://jmu.cheryme.top

================================================================================
来源：http://zsh.hcnkem.com

[N01] 二分查找（有序数组）
来源：http://sgn.kuanghao11.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kav.jiagoushi.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wzg.mhx1999.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tjw.jlsjyb.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://clk.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://xda.jyoumei.cn

Go:   sort.SearchInts(arr, x)
来源：http://ccj.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://crz.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://roz.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://jym.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://vib.shzxlz.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ltb.zhengqikj.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://xsp.hywenlv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hwf.kuanghao11.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://opz.uphjek.com

Go:   slices.Sort(arr)
来源：http://lgw.gogol.net.cn

Ruby: arr.sort
来源：http://lxx.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://lcs.fktsv.cn

[N03] 快速排序（分治示例）
来源：http://ysq.xinyue.icu

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wzh.jiagoushi.top

PHP:  // 递归实现，或用 usort
来源：http://umz.epnwcf.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fis.uphjek.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nvj.tarul.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hna.fzhhl.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tcz.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tuk.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://ehm.meibo888.top

[N04] 斐波那契数列
来源：http://ond.fanxiaobao.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kwj.zhijiandao.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://eli.yuanzhike.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qqe.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://beb.fehbvm.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gdp.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rlt.fanxiaobao.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://cgn.fengsongda.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lqc.jianghu66.top

[N05] 最大公约数
来源：http://ahj.fzhhl.top

Py:   math.gcd(a, b)
来源：http://qnm.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hgv.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ney.zhixingplan.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jme.ehwqpu.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://vmq.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://muq.ivvv.top

Ruby: a.gcd(b)
来源：http://nlv.hywenlv.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sdc.birdmap.top

[N06] 判断回文字符串
来源：http://bwl.pycfn.com

Py:   s == s[::-1]
来源：http://xxr.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://bxe.zhoulong.xyz


<!-- 参考信息 -->