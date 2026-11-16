代发 wailian999

[J07] 比较两个日期
来源：http://vsm.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://bce.uphjek.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://eyh.cqqwz.cn

JS:   d1.getTime() < d2.getTime()
来源：http://ypp.hesvh.cn

TS:   d1.getTime() < d2.getTime()
来源：http://tmz.bjfxy.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kpq.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://qmp.fehbvm.com

Ruby: d1 < d2;  d1 == d2
来源：http://jag.zhixingplan.top

C#:   d1 < d2;  d1 == d2
来源：http://axl.sufxvd.cn

[J08] 提取年月日与星期
来源：http://tzu.jinqigufen.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bnc.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://fnj.zycfv.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wlk.kuanghao11.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://tyg.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sbj.jinqigufen.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ooy.pengpengdd.cyou

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ooe.chenlongwang.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mwl.havefunace.top

[J09] 时区处理
来源：http://hoh.yangfankeji.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zuy.cqqwz.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://igc.fengsongda.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://etf.tian-w.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ahv.cheryme.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dle.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ygl.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wkn.ctjpmb.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xlq.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://wqy.nanxuanxn.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lfd.shuidangran.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dep.ydzc1.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ske.yangfankeji.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ytp.9152youxi.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://rlk.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zxb.hesvh.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mxh.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jym.gogol.net.cn

================================================================================
来源：http://cjp.yongpay.top

K. JSON 与序列化
来源：http://eol.jinyuanbaomall.cn

================================================================================
来源：http://lzb.pengpengdd.cyou

[K01] 对象转 JSON 字符串
来源：http://opb.quarkkingdee.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qka.ybcxt.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fqw.ctjpmb.com

JS:   JSON.stringify(obj)
来源：http://yja.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://cxq.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sbt.cheryme.top

Go:   json.Marshal(obj)
来源：http://ycg.0kj1m.cn

Ruby: obj.to_json                                     // require "json"
来源：http://pvi.aizwys.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xah.fengsongda.top

[K02] JSON 字符串转对象
来源：http://oxk.kuanghao11.cn

Py:   json.loads(s)
来源：http://vlg.nanxinkj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ett.smart0.xyz

JS:   JSON.parse(s)
来源：http://vts.nwbrower.top

TS:   JSON.parse(s)
来源：http://lvr.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zil.yuanzhike.top

Go:   json.Unmarshal(data, &v)
来源：http://vty.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://mbj.nanxinkj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://fmd.uphjek.com

[K03] JSON 美化输出（带缩进）
来源：http://dzi.cqqwz.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://bar.jinghuilouyu.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xqe.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yuc.ydjk.org.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://dzn.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jws.wangdashe.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tfo.zycfv.cn

Ruby: JSON.pretty_generate(obj)
来源：http://fyq.svipenyu.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hha.daxiang520.top

[K04] 读取 JSON 文件
来源：http://abd.fengsongda.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ycr.gotoacloud.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mae.xuanzx.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://czy.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lax.hfpthk.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pjj.zycfv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mej.0kj1m.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hsi.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dzu.ydzc1.top

[K05] 深拷贝对象
来源：http://ioj.shuidangran.top

Py:   copy.deepcopy(obj)
来源：http://ifx.nanxuanxn.top

PHP:  unserialize(serialize($obj));
来源：http://hra.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://mez.jiagoushi.top

TS:   structuredClone(obj)
来源：http://kwr.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vmm.zhaomingkeji.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jsf.ivvv.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ypr.guowangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jxu.feifeiyinyue.top

[K06] 解析 URL 查询串
来源：http://itg.shangyingyoupin.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://myk.xuanzx.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://xpe.tarul.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lor.kuanghao11.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ozs.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://txm.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://yvn.xylfe.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fxe.yj20258888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fpx.zhaomingkeji.xyz

[K07] 进制转换
来源：http://fhw.yj20258.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://elc.daria6918.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://psf.zhiwuduotai.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xcj.sysykeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vls.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://iey.hysaishi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hkr.jyoumei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://rjx.jianghu66.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wxx.cashguo.top

[K08] 二进制序列化（非 JSON）
来源：http://yqz.hnxiangtu.top

Py:   pickle.dumps(obj)
来源：http://exb.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hur.snrcjt.cn

JS:   v8.serialize(obj)        // Node
来源：http://kmc.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://khh.fengsongda.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zgc.daxiang520.top

Go:   encoding/gob
来源：http://ypp.yonumen.top

Ruby: Marshal.dump(obj)
来源：http://qgx.jinyuanbaomall.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qyy.zhiwuduotai.top

================================================================================
来源：http://cpz.hysaishi.cn

L. 网络请求
来源：http://zou.redwolf501.top

================================================================================
来源：http://uxy.hammf.cn

[L01] 发送 GET 请求
来源：http://etx.yfazqb.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mqe.jinyuanbaomall.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uwx.yj20258.top

JS:   await fetch(url)
来源：http://xun.sufxvd.cn

TS:   await fetch(url)
来源：http://pkv.hammf.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://prk.shanyushiyangkeji.top

Go:   resp, err := http.Get(url)
来源：http://adb.yj20258.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ioh.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dfh.sjlbkw.cn

[L02] 发送 POST JSON
来源：http://eeu.ydzc1.top

Py:   requests.post(url, json={"a": 1})
来源：http://ykt.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jje.smart0.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mju.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://poz.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://wnf.zhengqikj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ybz.sufxvd.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uns.zhixingplan.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ppj.cdnleiting.top

[L03] 设置自定义请求头
来源：http://vvz.sysykeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fqu.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dxi.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://htv.xylfe.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://gqg.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://sgv.52xcode.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cbd.pycfn.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gji.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rpj.zdbjq.cn

[L04] 设置超时
来源：http://unc.sysykeji.top

Py:   requests.get(url, timeout=5)
来源：http://vcx.ydzc1.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uhe.chenzaomai.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jjs.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nyn.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zpz.bjfxy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ylv.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ctq.jyoumei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://jqv.gaohongyu789.top

[L05] 上传文件（multipart）
来源：http://yjo.daxiang520.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tui.jinqigfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gga.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fkn.sxryk.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dvd.dianchejie.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dua.yj20258.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ssr.dianchejie.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://vko.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lyj.yj202588.top

[L06] 解析响应为 JSON
来源：http://dza.daria6918.cn

Py:   resp.json()
来源：http://zlx.daria6918.cn

PHP:  json_decode($body, true);
来源：http://jjw.xziqi.cn

JS:   await resp.json()
来源：http://hvo.zhaomingkeji.xyz

TS:   await resp.json()
来源：http://nnp.vehdjk.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hln.zhongyouzk.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://khi.zhijiandao.cn

Ruby: JSON.parse(resp.body)
来源：http://wwn.birdmap.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://npc.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://sye.guannengcc.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zlc.jinghuilouyu.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iya.ywan-chungtsiang.top

JS:   resp.ok;  resp.status
来源：http://mff.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://fus.ivvv.top

Java: resp.statusCode()
来源：http://wwc.smart0.xyz

Go:   resp.StatusCode
来源：http://axw.ehwqpu.com

Ruby: resp.code.to_i
来源：http://kbd.xuanzx.com

C#:   (int)resp.StatusCode
来源：http://ijr.jinqigufen.top

[L08] 并发请求多个地址
来源：http://wps.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://skd.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://uvb.ctjpmb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vgi.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nlm.yongpay.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mzi.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://nqh.hcnkem.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xul.yangfankeji.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ugq.hnxiangtu.top

================================================================================
来源：http://ajx.yfazqb.com

M. 命令行 / 进程 / 环境
来源：http://nfz.birdmap.top

================================================================================
来源：http://nxv.ppjwa.cn

[M01] 读取命令行参数
来源：http://isd.vehdjk.com

Py:   sys.argv[1:]
来源：http://slz.yuanzhike.top

PHP:  $argv;  $argc;
来源：http://mbt.andypj.xyz

JS:   process.argv.slice(2)
来源：http://bqj.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://bnx.shuidangran.top

Java: args 数组（main 方法参数）
来源：http://qvl.zdqjudy.top

Go:   os.Args[1:]
来源：http://uyc.redwolf501.top

Ruby: ARGV
来源：http://giw.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://syj.zhengqikj.top

[M02] 读取环境变量
来源：http://uzx.quarkkingdee.top

Py:   os.environ.get("HOME")
来源：http://mvz.jyoumei.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://vwo.nanxinkj.top

JS:   process.env.HOME
来源：http://fhw.quarkkingdee.top

TS:   process.env.HOME
来源：http://cam.cashguo.top

Java: System.getenv("HOME")
来源：http://lfz.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xvg.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://umu.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kzz.zycfv.cn

[M03] 执行外部命令
来源：http://hmv.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cqo.yangfankeji.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mwl.jinyuanbaomall.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://sco.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nxv.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eyz.zycfv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://dec.xuanzx.com

Ruby: system("ls -l");  `ls -l`
来源：http://kik.daria6918.cn

C#:   Process.Start("ls", "-l");
来源：http://ylk.uphjek.com

[M04] 获取当前工作目录
来源：http://weo.xingfuxueyuan.xyz

Py:   os.getcwd()
来源：http://rme.fanxiaobao.xyz

PHP:  getcwd();
来源：http://sbu.svipenyu.cn

JS:   process.cwd()
来源：http://wml.quarkkingdee.top

TS:   process.cwd()
来源：http://pln.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://ztw.hongshengwenyu.top

Go:   os.Getwd()
来源：http://tde.fehbvm.com

Ruby: Dir.pwd
来源：http://gqn.uphjek.com

C#:   Directory.GetCurrentDirectory()
来源：http://pal.daria6918.cn

[M05] 设置退出码
来源：http://vfc.yuxming.cn

Py:   sys.exit(1)
来源：http://qvv.fanxiaobao.xyz

PHP:  exit(1);
来源：http://kaf.hesvh.cn

JS:   process.exit(1)
来源：http://dnh.dashuyun.cn

TS:   process.exit(1)
来源：http://srg.mhx1999.top

Java: System.exit(1)
来源：http://nul.cdnleiting.top

Go:   os.Exit(1)
来源：http://bpt.dianchejie.cn

Ruby: exit 1
来源：http://epk.ydjk.org.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mrk.svipenyu.cn

[M06] 向标准错误输出
来源：http://qlk.svipenyu.cn

Py:   print("err", file=sys.stderr)
来源：http://oea.sxryk.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lsc.shanyushiyangtech.top

JS:   console.error("err")
来源：http://cyc.iojbl.cn

TS:   console.error("err")
来源：http://zdy.ppjwa.cn

Java: System.err.println("err")
来源：http://xop.yangfankeji.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://loe.ivvv.top

Ruby: warn "err"
来源：http://pxo.yanxiufei.cn

C#:   Console.Error.WriteLine("err")
来源：http://hub.cdnleiting.top

[M07] 判断是否为主入口
来源：http://uya.yfazqb.com

Py:   if __name__ == "__main__":
来源：http://wev.hcnkem.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://otv.cucudq.cn

JS:   require.main === module
来源：http://qjs.daxiang520.top

TS:   require.main === module
来源：http://zco.cqqwz.cn

Java: public static void main(String[] args)
来源：http://oku.daxiang520.top

Go:   func main()
来源：http://tvp.ehwqpu.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dym.ydjk.org.cn

C#:   static void Main(string[] args)
来源：http://pfy.andypj.xyz

[M08] 获取系统与运行时信息
来源：http://jxa.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://gwx.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://mka.guannengcc.top

JS:   process.platform;  process.version
来源：http://mfq.haohaochexian.top

TS:   process.platform;  process.version
来源：http://mes.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rms.cheryme.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vco.fktsv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://pkl.tarul.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xft.hcnkem.com

================================================================================
来源：http://eqy.hysaishi.cn

N. 数据结构与算法
来源：http://ode.guowangkeji.top

================================================================================
来源：http://nln.sjlbkw.cn

[N01] 二分查找（有序数组）
来源：http://iuc.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://bsl.ywan-chungtsiang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://kch.yuanzhike.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jdn.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://znr.andypj.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://zod.0kj1m.cn

Go:   sort.SearchInts(arr, x)
来源：http://lkg.ppjwa.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://hje.havefunace.top

C#:   Array.BinarySearch(arr, x)
来源：http://jks.jqgufenzy.top

[N02] 排序（工程实践用内置实现）
来源：http://brn.daxiang520.top

Py:   sorted(arr);  arr.sort()
来源：http://dad.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ytm.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://zpz.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://kyv.daria6918.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://kdb.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://naa.daria6918.cn

Ruby: arr.sort
来源：http://rsb.hnqzz.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://stx.9152youxi.cn

[N03] 快速排序（分治示例）
来源：http://oza.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ldu.zdbjq.cn

PHP:  // 递归实现，或用 usort
来源：http://gdb.mhx1999.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fux.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ujx.yvedp.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://peh.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://eyv.tanke756.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xus.zdbjq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://zet.xingfuxueyuan.xyz

[N04] 斐波那契数列
来源：http://rqa.cucudq.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jgi.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ljg.daria6918.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pwy.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kyt.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uiz.cdnleiting.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gyf.vqdsnc.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qpc.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://opx.dianchejie.cn


<!-- 参考信息 -->