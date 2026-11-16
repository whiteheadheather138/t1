代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://vfs.vehdjk.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://hms.haohaochexian.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://rtr.dashuyun.cn

Ruby: d1 < d2;  d1 == d2
来源：http://eob.hcnkem.com

C#:   d1 < d2;  d1 == d2
来源：http://rbi.0kj1m.cn

[J08] 提取年月日与星期
来源：http://qti.jlsjyb.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hoi.xuanzx.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xha.ybcxt.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://unt.shuidangran.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gzq.jlsjyb.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://izu.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://nxn.dianchejie.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uej.mhx1999.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wjf.jinghuilouyu.cn

[J09] 时区处理
来源：http://fyf.zdqjudy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://uqf.nanxinkj.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://syq.cashguo.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qin.cucudq.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://doc.yj20258.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ncy.dashuyun.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ngn.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://tdg.nwbrower.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ktm.sweek.top

[J10] 取今天 / 本月第一天
来源：http://tse.zhaomingkeji.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://sha.snrcjt.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hmx.fanxiaobao.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://wjx.dashuyun.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ogt.gogol.net.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ngw.ppjwa.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://scr.tanke756.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vmb.nanxuanxn.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uxs.jqgufenzy.top

================================================================================
来源：http://rzm.guannengcc.top

K. JSON 与序列化
来源：http://cby.jqgufenzy.top

================================================================================
来源：http://lio.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://tov.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://tos.yanxiufei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ncp.cashguo.top

JS:   JSON.stringify(obj)
来源：http://lne.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://juo.daria6918.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kpi.quarkkingdee.top

Go:   json.Marshal(obj)
来源：http://urf.yj20258.top

Ruby: obj.to_json                                     // require "json"
来源：http://vmn.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lgh.ywan-chungtsiang.top

[K02] JSON 字符串转对象
来源：http://qim.sufxvd.cn

Py:   json.loads(s)
来源：http://xip.mhx1999.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vgz.hongshengwenyu.top

JS:   JSON.parse(s)
来源：http://uol.ctjpmb.com

TS:   JSON.parse(s)
来源：http://aav.fehbvm.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://cnt.dashuyun.cn

Go:   json.Unmarshal(data, &v)
来源：http://wbl.zycfv.cn

Ruby: JSON.parse(s)
来源：http://gxf.shzxlz.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://eni.pengpengdd.cyou

[K03] JSON 美化输出（带缩进）
来源：http://lgx.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://njd.hesvh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xso.chenzaomai.com

JS:   JSON.stringify(obj, null, 2)
来源：http://nup.xuetiantiany.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://wdd.316326.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://poi.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gkb.aibaodan.cn

Ruby: JSON.pretty_generate(obj)
来源：http://noz.jinqigufen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dok.andypj.xyz

[K04] 读取 JSON 文件
来源：http://oen.cheryme.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cso.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yya.ydzc1.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xtp.zdqjudy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://scn.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://bdb.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wnw.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://abq.52xcode.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wvu.zdbjq.cn

[K05] 深拷贝对象
来源：http://gyb.sweek.top

Py:   copy.deepcopy(obj)
来源：http://wvw.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://iby.chenlongwang.top

JS:   structuredClone(obj)
来源：http://vnz.aibaodan.cn

TS:   structuredClone(obj)
来源：http://jkr.zhaomingkeji.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://mso.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nag.dianchejie.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lpg.nwbrower.top

C#:   // 序列化往返，或自定义 Clone
来源：http://rdg.nanxuanxn.top

[K06] 解析 URL 查询串
来源：http://vnh.chenlongwang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://iuk.yfazqb.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://dbm.c1oappe.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xtv.dianchejie.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yxe.sxryk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vxq.epnwcf.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://vmq.feifeiyinyue.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://azg.0kj1m.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tvm.hfpthk.cn

[K07] 进制转换
来源：http://knc.zdbjq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qut.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://edt.bbcook.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lsv.vqdsnc.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://odk.xinyue.icu

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lix.yanxiufei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://fpx.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://clf.snrcjt.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ofj.chenlongwang.top

[K08] 二进制序列化（非 JSON）
来源：http://fwt.uphjek.com

Py:   pickle.dumps(obj)
来源：http://qyk.tanke756.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qgs.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://rcg.yonumen.top

TS:   v8.serialize(obj)        // Node
来源：http://nvz.hnqzz.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ahi.shzxlz.cn

Go:   encoding/gob
来源：http://isp.nanxuanxn.top

Ruby: Marshal.dump(obj)
来源：http://pae.zhixingplan.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rdf.shzxlz.cn

================================================================================
来源：http://kgn.vehdjk.com

L. 网络请求
来源：http://psj.jinyuanbaomall.cn

================================================================================
来源：http://twh.cqqwz.cn

[L01] 发送 GET 请求
来源：http://csz.gotoacloud.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vwf.redwolf501.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ctk.jinyuanbaomall.cn

JS:   await fetch(url)
来源：http://oje.havefunace.top

TS:   await fetch(url)
来源：http://cgk.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mnx.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://gck.jianghu66.top

Ruby: Net::HTTP.get(URI(url))
来源：http://htb.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://son.zhoulong.xyz

[L02] 发送 POST JSON
来源：http://lka.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ulg.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ruv.yj202588.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://aiz.ywan-chungtsiang.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ful.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gyq.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vny.birdmap.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qkq.smart0.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hus.jinqigfzy.top

[L03] 设置自定义请求头
来源：http://mvy.ydzc1.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lfs.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yek.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pkz.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hkt.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xgb.ywan-chungtsiang.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zsw.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vsy.xuetiantiany.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://csg.gaohongyu789.top

[L04] 设置超时
来源：http://xzs.hesvh.cn

Py:   requests.get(url, timeout=5)
来源：http://nsx.yj20258.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ewq.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xlq.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://knh.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mjd.jlsjyb.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://jxm.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kbj.sxryk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://uty.sxryk.cn

[L05] 上传文件（multipart）
来源：http://nkm.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hha.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ffs.ctjpmb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://pli.birdmap.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jmg.yvedp.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://azx.316326.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ocx.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lhw.sweek.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://yql.hesvh.cn

[L06] 解析响应为 JSON
来源：http://aqc.wangshuangyany.cn

Py:   resp.json()
来源：http://bvs.bbcook.cn

PHP:  json_decode($body, true);
来源：http://rsp.andypj.xyz

JS:   await resp.json()
来源：http://gsj.pengpengdd.cyou

TS:   await resp.json()
来源：http://kpl.yj202588.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://edv.yangfankeji.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qqt.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://kam.yuanzhike.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ppw.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://avs.cheryme.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bia.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://uwl.andypj.xyz

JS:   resp.ok;  resp.status
来源：http://hve.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://dkg.ppjwa.cn

Java: resp.statusCode()
来源：http://ikk.cashguo.top

Go:   resp.StatusCode
来源：http://zyr.hcnkem.com

Ruby: resp.code.to_i
来源：http://tso.yueranfly.top

C#:   (int)resp.StatusCode
来源：http://flb.meibo888.top

[L08] 并发请求多个地址
来源：http://irx.tian-w.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cnr.ydjk.org.cn

PHP:  curl_multi_init() 系列
来源：http://rbh.cucudq.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wre.hnqzz.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fif.haohaochexian.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://gtg.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vvi.tianlin.xyz

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://odk.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://try.hnqzz.top

================================================================================
来源：http://zrc.jinyuanbaomall.cn

M. 命令行 / 进程 / 环境
来源：http://omc.zhiwuduotai.top

================================================================================
来源：http://egs.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://dvf.ehwqpu.com

Py:   sys.argv[1:]
来源：http://nfr.52xcode.cn

PHP:  $argv;  $argc;
来源：http://ibv.zycfv.cn

JS:   process.argv.slice(2)
来源：http://swq.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://jyg.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://vfy.meibo888.top

Go:   os.Args[1:]
来源：http://prn.xuetiantiany.cn

Ruby: ARGV
来源：http://hcl.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://foc.mhx1999.top

[M02] 读取环境变量
来源：http://dzo.pycfn.com

Py:   os.environ.get("HOME")
来源：http://bqp.haohaochexian.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fvw.fanxiaobao.xyz

JS:   process.env.HOME
来源：http://hrr.epnwcf.com

TS:   process.env.HOME
来源：http://ugx.haohaochexian.top

Java: System.getenv("HOME")
来源：http://emd.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vys.tianlin.xyz

Ruby: ENV["HOME"]
来源：http://mqb.pengpengdd.cyou

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://zji.shanyushiyangtech.top

[M03] 执行外部命令
来源：http://wnl.aibaodan.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://byb.yueranfly.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://reu.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pxs.bbcook.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oup.ydzc1.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wyg.0kj1m.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ywd.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://rqy.xylfe.cn

C#:   Process.Start("ls", "-l");
来源：http://mpg.ctjpmb.com

[M04] 获取当前工作目录
来源：http://xwa.tarul.cn

Py:   os.getcwd()
来源：http://zla.jianghu66.top

PHP:  getcwd();
来源：http://qjq.fanxiaobao.xyz

JS:   process.cwd()
来源：http://lvv.tianlin.xyz

TS:   process.cwd()
来源：http://nvo.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://wqi.jinyuanbaomall.cn

Go:   os.Getwd()
来源：http://sey.ybcxt.top

Ruby: Dir.pwd
来源：http://eqq.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://hlp.andypj.xyz

[M05] 设置退出码
来源：http://jvt.ppjwa.cn

Py:   sys.exit(1)
来源：http://mvt.birdmap.top

PHP:  exit(1);
来源：http://vsl.nanxuanxn.top

JS:   process.exit(1)
来源：http://lox.feifeiyinyue.top

TS:   process.exit(1)
来源：http://kam.chenlongwang.top

Java: System.exit(1)
来源：http://zon.ctjpmb.com

Go:   os.Exit(1)
来源：http://kjz.316326.xyz

Ruby: exit 1
来源：http://qwd.c1oappe.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ano.wangdashe.top

[M06] 向标准错误输出
来源：http://upo.wangdashe.top

Py:   print("err", file=sys.stderr)
来源：http://qyj.smart0.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://imh.yuxming.cn

JS:   console.error("err")
来源：http://rob.havefunace.top

TS:   console.error("err")
来源：http://mic.yfazqb.com

Java: System.err.println("err")
来源：http://zfv.cucudq.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://okc.9152youxi.cn

Ruby: warn "err"
来源：http://dqw.316326.xyz

C#:   Console.Error.WriteLine("err")
来源：http://ler.ydzc1.top

[M07] 判断是否为主入口
来源：http://lfq.redwolf501.top

Py:   if __name__ == "__main__":
来源：http://ldb.fanxiaobao.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gcm.yueranfly.top

JS:   require.main === module
来源：http://bfm.zdqjudy.top

TS:   require.main === module
来源：http://gyf.zhiwuduotai.top

Java: public static void main(String[] args)
来源：http://lzr.cqqwz.cn

Go:   func main()
来源：http://mko.jqgfzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tag.fengsongda.top

C#:   static void Main(string[] args)
来源：http://ywr.aibaodan.cn

[M08] 获取系统与运行时信息
来源：http://krm.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://tdj.shuidangran.top

PHP:  PHP_OS;  phpversion();
来源：http://caf.quarkkingdee.top

JS:   process.platform;  process.version
来源：http://dkz.ydjk.org.cn

TS:   process.platform;  process.version
来源：http://ymy.vehdjk.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://spa.bjfxy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tyh.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sjl.ybcxt.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kdm.yuxming.cn

================================================================================
来源：http://obk.quarkkingdee.top

N. 数据结构与算法
来源：http://vbu.svipenyu.cn

================================================================================
来源：http://pqg.nwbrower.top

[N01] 二分查找（有序数组）
来源：http://vnp.yj20258.top

Py:   bisect.bisect_left(arr, x)
来源：http://vav.andypj.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rbt.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lqg.tanke756.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mbn.shanyushiyangtech.top

Java: Arrays.binarySearch(arr, x)
来源：http://tgk.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://pvn.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://erw.sweek.top

C#:   Array.BinarySearch(arr, x)
来源：http://vod.jinyuanbaomall.cn

[N02] 排序（工程实践用内置实现）
来源：http://wud.zhijiandao.cn

Py:   sorted(arr);  arr.sort()
来源：http://gkf.tanke756.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hbz.cashguo.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ymg.xuanzx.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://esq.cucudq.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://swy.zhongyouzk.top

Go:   slices.Sort(arr)
来源：http://rvd.ppjwa.cn

Ruby: arr.sort
来源：http://uev.0kj1m.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://vxu.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://pdz.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://zha.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://udd.fktsv.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xxt.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mmg.sjlbkw.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dxq.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://trm.nanxuanxn.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yfs.zhongyouzk.top

C#:   // 手写递归，或 Array.Sort
来源：http://lhq.ybcxt.top

[N04] 斐波那契数列
来源：http://urr.jianghu66.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gki.ppjwa.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://boy.zhongyouzk.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://msi.0kj1m.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kmp.jinqigfzy.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://eyi.jinqigfzy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gxg.chenzaomai.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iot.cashguo.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://loo.yuxming.cn

[N05] 最大公约数
来源：http://gpl.haohaochexian.top

Py:   math.gcd(a, b)
来源：http://dxc.epnwcf.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://lkd.hfpthk.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wvu.zhoulong.xyz


<!-- 参考信息 -->