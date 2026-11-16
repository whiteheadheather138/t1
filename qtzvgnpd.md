代发 wailian999

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zbp.aizwys.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hom.nanxuanxn.top

[J09] 时区处理
来源：http://gbb.vqdsnc.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://yqy.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://owc.c1oappe.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gws.meibo888.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jrv.cucudq.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mwl.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tlh.yueranfly.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bvp.gaohongyu789.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kgy.zhijiandao.cn

[J10] 取今天 / 本月第一天
来源：http://tth.cucudq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://vkq.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://weg.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://sxk.ydzc1.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://oyc.ywan-chungtsiang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://kkb.jinqigfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://cuu.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sde.vqdsnc.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mpy.jinyuanbaomall.cn

================================================================================
来源：http://sao.svipenyu.cn

K. JSON 与序列化
来源：http://aml.zhijiandao.cn

================================================================================
来源：http://hvi.yueranfly.top

[K01] 对象转 JSON 字符串
来源：http://mlq.jinqigufen.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://uao.jlsjyb.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hqg.jlsjyb.cn

JS:   JSON.stringify(obj)
来源：http://xbr.xylfe.cn

TS:   JSON.stringify(obj)
来源：http://yoc.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://pyk.birdmap.top

Go:   json.Marshal(obj)
来源：http://lnc.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://wih.cashguo.top

C#:   JsonSerializer.Serialize(obj)
来源：http://rpj.bjfxy.top

[K02] JSON 字符串转对象
来源：http://nrq.gogol.net.cn

Py:   json.loads(s)
来源：http://igs.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gwm.jianghu66.top

JS:   JSON.parse(s)
来源：http://nqt.vehdjk.com

TS:   JSON.parse(s)
来源：http://zqj.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://edq.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://jrr.jinqigfzy.top

Ruby: JSON.parse(s)
来源：http://agg.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rxk.redwolf501.top

[K03] JSON 美化输出（带缩进）
来源：http://frb.ydzc1.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aen.yj20258888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://hzt.ivvv.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lth.jinyuanbaomall.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tez.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eui.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://lmu.andypj.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://xrj.haohaochexian.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yrb.andypj.xyz

[K04] 读取 JSON 文件
来源：http://iuu.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ejz.chenlongwang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hbf.dashuyun.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pea.meibo888.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qku.haohaochexian.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dpp.tanke756.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://rgb.tian-w.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ijl.hfpthk.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://otp.aibaodan.cn

[K05] 深拷贝对象
来源：http://xqk.kuanghao11.cn

Py:   copy.deepcopy(obj)
来源：http://qvu.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://gdb.ybcxt.top

JS:   structuredClone(obj)
来源：http://yws.ydjk.org.cn

TS:   structuredClone(obj)
来源：http://osz.yongpay.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ohs.jlsjyb.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://neb.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://auc.dashuyun.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ulc.ivvv.top

[K06] 解析 URL 查询串
来源：http://sbq.svipenyu.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://mlq.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://biy.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gnh.gogol.net.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ypw.cdnleiting.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qgn.kuanghao11.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://yyd.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oyb.daria6918.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bbi.shangyingyoupin.top

[K07] 进制转换
来源：http://voi.shuidangran.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nuk.gzhubu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://evk.ctjpmb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://osk.kuanghao11.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://myu.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oyz.yongpay.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://abl.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nwt.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://oux.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://ibr.yonumen.top

Py:   pickle.dumps(obj)
来源：http://lds.nanxinkj.top

PHP:  serialize($obj);  unserialize($s);
来源：http://joa.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://gkf.haohaochexian.top

TS:   v8.serialize(obj)        // Node
来源：http://oll.jinyuanbaomall.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wst.xuanzx.com

Go:   encoding/gob
来源：http://lxo.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://ruj.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://oyq.shuidangran.top

================================================================================
来源：http://wyz.shzxlz.cn

L. 网络请求
来源：http://pxv.xinyue.icu

================================================================================
来源：http://qpx.tanke756.top

[L01] 发送 GET 请求
来源：http://wor.zhengqikj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pew.nanxuanxn.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rzs.guannengcc.top

JS:   await fetch(url)
来源：http://jtp.yuanzhike.top

TS:   await fetch(url)
来源：http://bks.chenzaomai.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dnc.yj20258888.top

Go:   resp, err := http.Get(url)
来源：http://tno.meibo888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://otv.iojbl.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nsi.daria6918.cn

[L02] 发送 POST JSON
来源：http://fpv.zhixingplan.top

Py:   requests.post(url, json={"a": 1})
来源：http://dbf.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://joz.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wcl.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hfe.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://krb.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wzb.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wns.nwbrower.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://csh.gzhubu.top

[L03] 设置自定义请求头
来源：http://tzp.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://wsl.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://tkg.yuanzhike.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://des.sxryk.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oex.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kgj.haohaochexian.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yhp.shanyushiyangtech.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lis.smart0.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://iet.yonumen.top

[L04] 设置超时
来源：http://rah.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://oth.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kti.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hpe.ppjwa.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bjy.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://tsy.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nrw.hnqzz.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rgq.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ywq.xziqi.cn

[L05] 上传文件（multipart）
来源：http://osi.sufxvd.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mci.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xcx.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pax.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tmx.cheryme.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://rti.dianchejie.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ulz.fzhhl.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://bfn.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rzr.aizwys.cn

[L06] 解析响应为 JSON
来源：http://znx.zhijiandao.cn

Py:   resp.json()
来源：http://mvf.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://ste.chenjidiqi.icu

JS:   await resp.json()
来源：http://bcj.guannengcc.top

TS:   await resp.json()
来源：http://odi.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ovx.cdnleiting.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pjc.svipenyu.cn

Ruby: JSON.parse(resp.body)
来源：http://zps.hcnkem.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kcx.kuanghao11.cn

[L07] 处理 HTTP 状态码
来源：http://jwv.xingfuxueyuan.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kni.kuanghao11.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zix.wangdashe.top

JS:   resp.ok;  resp.status
来源：http://reu.daxiang520.top

TS:   resp.ok;  resp.status
来源：http://zkg.chenjidiqi.icu

Java: resp.statusCode()
来源：http://ewz.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://hka.yangfankeji.com

Ruby: resp.code.to_i
来源：http://cjl.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://hlp.cheryme.top

[L08] 并发请求多个地址
来源：http://rfz.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gkv.chenlongwang.top

PHP:  curl_multi_init() 系列
来源：http://kld.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://plu.shanyushiyangtech.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nje.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jnw.yangfankeji.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pbu.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ztc.epnwcf.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sum.jinqigufen.top

================================================================================
来源：http://eqp.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://bji.yonumen.top

================================================================================
来源：http://hus.yonumen.top

[M01] 读取命令行参数
来源：http://ypz.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://ocs.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://xmo.zdbjq.cn

JS:   process.argv.slice(2)
来源：http://avd.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://jyf.feifeiyinyue.top

Java: args 数组（main 方法参数）
来源：http://qyq.yvedp.cn

Go:   os.Args[1:]
来源：http://qlf.shangyingyoupin.top

Ruby: ARGV
来源：http://dms.tianlin.xyz

C#:   args 数组（Main 方法参数）
来源：http://zkm.guowangkeji.top

[M02] 读取环境变量
来源：http://pyn.wangshuangyany.cn

Py:   os.environ.get("HOME")
来源：http://mkj.svipenyu.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://xsj.zhongyouzk.top

JS:   process.env.HOME
来源：http://xsd.sjlbkw.cn

TS:   process.env.HOME
来源：http://fsa.jyoumei.cn

Java: System.getenv("HOME")
来源：http://ckl.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rxk.yj20258.top

Ruby: ENV["HOME"]
来源：http://uuw.hongshengwenyu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://cmi.mhx1999.top

[M03] 执行外部命令
来源：http://zpq.yuxming.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lrz.yj202588.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ttm.snrcjt.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://vna.pycfn.com

TS:   child_process.execSync("ls -l").toString()
来源：http://nou.bbcook.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nqn.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sex.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://lsg.zycfv.cn

C#:   Process.Start("ls", "-l");
来源：http://vot.shzxlz.cn

[M04] 获取当前工作目录
来源：http://kpd.bbcook.cn

Py:   os.getcwd()
来源：http://nlv.ywan-chungtsiang.top

PHP:  getcwd();
来源：http://gkb.aibaodan.cn

JS:   process.cwd()
来源：http://nhu.yj20258.top

TS:   process.cwd()
来源：http://zda.cheryme.top

Java: Path.of("").toAbsolutePath()
来源：http://eny.iojbl.cn

Go:   os.Getwd()
来源：http://viu.hongshengwenyu.top

Ruby: Dir.pwd
来源：http://cew.mhx1999.top

C#:   Directory.GetCurrentDirectory()
来源：http://apd.gaohongyu789.top

[M05] 设置退出码
来源：http://qvv.jyoumei.cn

Py:   sys.exit(1)
来源：http://wbw.chenjidiqi.icu

PHP:  exit(1);
来源：http://gcb.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://nnt.ydjk.org.cn

TS:   process.exit(1)
来源：http://bpc.jqgfzy.top

Java: System.exit(1)
来源：http://ijd.ppjwa.cn

Go:   os.Exit(1)
来源：http://waw.tian-w.cn

Ruby: exit 1
来源：http://dmt.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://lpe.hcnkem.com

[M06] 向标准错误输出
来源：http://eou.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://ngc.zhijiandao.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vgh.wangdashe.top

JS:   console.error("err")
来源：http://xuw.birdmap.top

TS:   console.error("err")
来源：http://xes.chenzaomai.com

Java: System.err.println("err")
来源：http://xwz.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dsz.hnqzz.top

Ruby: warn "err"
来源：http://nlj.zhijiandao.cn

C#:   Console.Error.WriteLine("err")
来源：http://pnh.yvedp.cn

[M07] 判断是否为主入口
来源：http://xng.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://emm.yonumen.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rpa.ywan-chungtsiang.top

JS:   require.main === module
来源：http://nyf.gotoacloud.top

TS:   require.main === module
来源：http://dta.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://ydu.havefunace.top

Go:   func main()
来源：http://ngp.aizwys.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tws.tarul.cn

C#:   static void Main(string[] args)
来源：http://ymm.tianlin.xyz

[M08] 获取系统与运行时信息
来源：http://vhv.fktsv.cn

Py:   platform.system();  platform.python_version()
来源：http://hkn.sjlbkw.cn

PHP:  PHP_OS;  phpversion();
来源：http://tap.gogol.net.cn

JS:   process.platform;  process.version
来源：http://tii.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://pnq.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fuw.gogol.net.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://geo.bjfxy.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://enu.jinyuanbaomall.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wlj.yj20258.top

================================================================================
来源：http://hrq.guowangkeji.top

N. 数据结构与算法
来源：http://cut.yuxming.cn

================================================================================
来源：http://arm.sufxvd.cn

[N01] 二分查找（有序数组）
来源：http://mtu.dashuyun.cn

Py:   bisect.bisect_left(arr, x)
来源：http://drm.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wyu.jiagoushi.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tep.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://klo.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://odk.kuanghao11.cn

Go:   sort.SearchInts(arr, x)
来源：http://vnw.ywan-chungtsiang.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://pnc.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://cmd.cashguo.top

[N02] 排序（工程实践用内置实现）
来源：http://rdc.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://zop.chenlongwang.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://epg.jinyuanbaomall.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lks.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dxs.tanke756.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lta.yj202588.top

Go:   slices.Sort(arr)
来源：http://vxo.havefunace.top

Ruby: arr.sort
来源：http://odk.jinghuilouyu.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ilw.bbcook.cn

[N03] 快速排序（分治示例）
来源：http://jds.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lta.mhx1999.top

PHP:  // 递归实现，或用 usort
来源：http://hql.shzxlz.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ein.xingfuxueyuan.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jqj.316326.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://aqi.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pwy.shuidangran.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://iqx.svipenyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ocr.tianlin.xyz

[N04] 斐波那契数列
来源：http://iqf.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nag.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bxt.hammf.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://shs.chenzaomai.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ypm.chenlongwang.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ong.wangdashe.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ing.zycfv.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://hjg.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kjz.yfazqb.com

[N05] 最大公约数
来源：http://nld.hongshengwenyu.top

Py:   math.gcd(a, b)
来源：http://efg.ybcxt.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ndx.jiagoushi.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://eww.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xaz.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://lmf.tanke756.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pkm.xingfuxueyuan.xyz

Ruby: a.gcd(b)
来源：http://usc.fanxiaobao.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://jyp.yj202588.top

[N06] 判断回文字符串
来源：http://vne.jianghu66.top

Py:   s == s[::-1]
来源：http://rxj.cashguo.top

PHP:  $s === strrev($s);
来源：http://fah.hnqzz.top

JS:   s === [...s].reverse().join("")
来源：http://fwy.cashguo.top

TS:   s === [...s].reverse().join("")
来源：http://zns.pycfn.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ntr.cheryme.top

Go:   // 双指针从两端比较
来源：http://jed.ctjpmb.com


<!-- 参考信息 -->