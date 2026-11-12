代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://rbm.xinyue.icu

Go:   end.Sub(start).Hours()
来源：http://dbb.cqqwz.cn

Ruby: end - start                 # 返回秒数
来源：http://das.jqgfzy.top

C#:   (end - start).TotalSeconds
来源：http://bci.fanxiaobao.xyz

[J07] 比较两个日期
来源：http://zar.jlsjyb.cn

Py:   d1 < d2;  d1 == d2
来源：http://qbb.yueranfly.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://dde.tianlin.xyz

JS:   d1.getTime() < d2.getTime()
来源：http://jcv.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://dhi.andypj.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gnj.sweek.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://wlw.316326.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://goa.daria6918.cn

C#:   d1 < d2;  d1 == d2
来源：http://ion.yj20258888.top

[J08] 提取年月日与星期
来源：http://nxt.ppjwa.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rup.cucudq.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://eqf.meibo888.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://sbc.chenzaomai.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aul.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ypu.havefunace.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gut.yonumen.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lml.tanke756.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dsw.pengpengdd.cyou

[J09] 时区处理
来源：http://ldo.hywenlv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://won.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://edv.havefunace.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://srz.pengpengdd.cyou

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mbv.yangfankeji.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ioq.yonumen.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oqw.zhijiandao.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://zgt.fktsv.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://iku.cdnleiting.top

[J10] 取今天 / 本月第一天
来源：http://nqr.yongpay.top

Py:   date.today();  date.today().replace(day=1)
来源：http://uth.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nhc.nanxuanxn.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kyn.quarkkingdee.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fyg.cqqwz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qfb.xuetiantiany.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://emo.cashguo.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://uad.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jjz.9152youxi.cn

================================================================================
来源：http://jgc.yueranfly.top

K. JSON 与序列化
来源：http://dpj.mhx1999.top

================================================================================
来源：http://tct.zhoulong.xyz

[K01] 对象转 JSON 字符串
来源：http://zeb.xylfe.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ead.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ycm.hcnkem.com

JS:   JSON.stringify(obj)
来源：http://jfs.zhaomingkeji.xyz

TS:   JSON.stringify(obj)
来源：http://auh.gaohongyu789.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://gyl.gaohongyu789.top

Go:   json.Marshal(obj)
来源：http://grb.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://zfh.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://mju.shangyingyoupin.top

[K02] JSON 字符串转对象
来源：http://lhz.guannengcc.top

Py:   json.loads(s)
来源：http://pvv.jianghu66.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tiu.gzhubu.top

JS:   JSON.parse(s)
来源：http://mkg.redwolf501.top

TS:   JSON.parse(s)
来源：http://evr.jinyuanbaomall.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://eei.nanxinkj.top

Go:   json.Unmarshal(data, &v)
来源：http://pzn.yangfankeji.com

Ruby: JSON.parse(s)
来源：http://hgn.quarkkingdee.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qut.gzhubu.top

[K03] JSON 美化输出（带缩进）
来源：http://yms.hcnkem.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yac.gotoacloud.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pzn.gotoacloud.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xsu.quarkkingdee.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ojh.tanke756.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bbg.shuidangran.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hwk.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://jel.jiagoushi.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hjz.xingfuxueyuan.xyz

[K04] 读取 JSON 文件
来源：http://rkc.vehdjk.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wic.hfpthk.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ffb.hywenlv.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ssm.yueranfly.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lrr.kuanghao11.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fhd.yuanzhike.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fis.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tes.bjfxy.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ekh.pycfn.com

[K05] 深拷贝对象
来源：http://pdf.ybcxt.top

Py:   copy.deepcopy(obj)
来源：http://vgf.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://bad.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://vss.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://bhw.tian-w.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ghm.hywenlv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://toj.ydzc1.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jeu.jyoumei.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aiz.jqgufenzy.top

[K06] 解析 URL 查询串
来源：http://rke.uphjek.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nlk.yj202588.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yag.yj202588.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rtw.yj20258.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pug.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gfj.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uqb.shuidangran.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://sdw.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wgq.cashguo.top

[K07] 进制转换
来源：http://inh.hnxiangtu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vdl.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pxg.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://nas.gaohongyu789.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xra.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ozv.shuidangran.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ubx.chenzaomai.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://meo.fengsongda.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://eid.dashuyun.cn

[K08] 二进制序列化（非 JSON）
来源：http://dop.cdnleiting.top

Py:   pickle.dumps(obj)
来源：http://ftf.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://bvd.hesvh.cn

JS:   v8.serialize(obj)        // Node
来源：http://zhf.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://nom.ydjk.org.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uco.ivvv.top

Go:   encoding/gob
来源：http://mib.zhixingplan.top

Ruby: Marshal.dump(obj)
来源：http://xvk.hfpthk.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sxn.sysykeji.top

================================================================================
来源：http://lnd.guannengcc.top

L. 网络请求
来源：http://yie.ppjwa.cn

================================================================================
来源：http://fda.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://vat.meibo888.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://szk.cucudq.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://hxw.shanyushiyangtech.top

JS:   await fetch(url)
来源：http://eft.chenjidiqi.icu

TS:   await fetch(url)
来源：http://wny.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ojs.zhiwuduotai.top

Go:   resp, err := http.Get(url)
来源：http://bdl.gaohongyu789.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jpc.ivvv.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bkh.andypj.xyz

[L02] 发送 POST JSON
来源：http://fzk.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://kcl.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yal.svipenyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qln.yfazqb.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wps.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://eqn.hnqzz.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lhz.cqqwz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tvr.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://giq.xuanzx.com

[L03] 设置自定义请求头
来源：http://asf.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fkx.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://euk.quarkkingdee.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ctj.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lwo.aibaodan.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kuw.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://khu.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bxz.zdbjq.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ezx.hywenlv.cn

[L04] 设置超时
来源：http://shw.fzhhl.top

Py:   requests.get(url, timeout=5)
来源：http://rqf.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://cxt.iojbl.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://muk.c1oappe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fvy.jyoumei.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://scq.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nus.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ljk.nanxuanxn.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://spl.hongshengwenyu.top

[L05] 上传文件（multipart）
来源：http://hdz.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vxd.birdmap.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qbf.fktsv.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lon.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mjs.cqqwz.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nrc.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://zct.pengpengdd.cyou

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oyo.fktsv.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gfl.zhijiandao.cn

[L06] 解析响应为 JSON
来源：http://isb.cheryme.top

Py:   resp.json()
来源：http://hgq.zdbjq.cn

PHP:  json_decode($body, true);
来源：http://edp.havefunace.top

JS:   await resp.json()
来源：http://fqh.jinqigfzy.top

TS:   await resp.json()
来源：http://ygg.nwbrower.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pbc.tarul.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://zig.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://ecg.wangshuangyany.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rro.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://yzw.hnxiangtu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://whz.feifeiyinyue.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mmh.tanke756.top

JS:   resp.ok;  resp.status
来源：http://aym.yuxming.cn

TS:   resp.ok;  resp.status
来源：http://vqh.fzhhl.top

Java: resp.statusCode()
来源：http://iui.jinyuanbaomall.cn

Go:   resp.StatusCode
来源：http://pnx.daxiang520.top

Ruby: resp.code.to_i
来源：http://wps.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://zrv.yueranfly.top

[L08] 并发请求多个地址
来源：http://feu.xinyue.icu

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://mtu.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://rbv.jiagoushi.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ymd.nwbrower.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vug.tianlin.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://hlm.xziqi.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://oxg.jinyuanbaomall.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tsv.zhixingplan.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jiy.guowangkeji.top

================================================================================
来源：http://krx.yvedp.cn

M. 命令行 / 进程 / 环境
来源：http://odp.ybcxt.top

================================================================================
来源：http://oze.vehdjk.com

[M01] 读取命令行参数
来源：http://tyh.jqgufenzy.top

Py:   sys.argv[1:]
来源：http://prc.epnwcf.com

PHP:  $argv;  $argc;
来源：http://vzv.shangyingyoupin.top

JS:   process.argv.slice(2)
来源：http://tpm.yonumen.top

TS:   process.argv.slice(2)
来源：http://cvj.meibo888.top

Java: args 数组（main 方法参数）
来源：http://mnc.yj20258.top

Go:   os.Args[1:]
来源：http://tko.ydjk.org.cn

Ruby: ARGV
来源：http://hoz.pycfn.com

C#:   args 数组（Main 方法参数）
来源：http://dag.hnqzz.top

[M02] 读取环境变量
来源：http://bwj.xylfe.cn

Py:   os.environ.get("HOME")
来源：http://ytf.zhoulong.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eny.ydjk.org.cn

JS:   process.env.HOME
来源：http://has.aibaodan.cn

TS:   process.env.HOME
来源：http://pns.hysaishi.cn

Java: System.getenv("HOME")
来源：http://mcs.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tcp.nwbrower.top

Ruby: ENV["HOME"]
来源：http://dyz.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://esh.hesvh.cn

[M03] 执行外部命令
来源：http://cqq.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://uoh.dashuyun.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://vyz.vqdsnc.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://owg.sjlbkw.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://whf.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://aeu.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nhm.fzhhl.top

Ruby: system("ls -l");  `ls -l`
来源：http://rne.gotoacloud.top

C#:   Process.Start("ls", "-l");
来源：http://poz.sjlbkw.cn

[M04] 获取当前工作目录
来源：http://vul.hfpthk.cn

Py:   os.getcwd()
来源：http://xrs.zhengqikj.top

PHP:  getcwd();
来源：http://rap.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://glh.aibaodan.cn

TS:   process.cwd()
来源：http://gvw.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://jvk.hfpthk.cn

Go:   os.Getwd()
来源：http://vir.smart0.xyz

Ruby: Dir.pwd
来源：http://pvf.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://rzd.snrcjt.cn

[M05] 设置退出码
来源：http://oug.nanxinkj.top

Py:   sys.exit(1)
来源：http://eno.ppjwa.cn

PHP:  exit(1);
来源：http://isv.jiagoushi.top

JS:   process.exit(1)
来源：http://jrz.jiagoushi.top

TS:   process.exit(1)
来源：http://fbb.havefunace.top

Java: System.exit(1)
来源：http://xyo.fengsongda.top

Go:   os.Exit(1)
来源：http://lkw.cucudq.cn

Ruby: exit 1
来源：http://ujv.jinghuilouyu.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kzu.bjfxy.top

[M06] 向标准错误输出
来源：http://ain.fzhhl.top

Py:   print("err", file=sys.stderr)
来源：http://xea.zhongyouzk.top

PHP:  fwrite(STDERR, "err\n");
来源：http://etm.xinyue.icu

JS:   console.error("err")
来源：http://fwv.yj202588.top

TS:   console.error("err")
来源：http://ban.gaohongyu789.top

Java: System.err.println("err")
来源：http://tce.xinyue.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yhe.kuanghao11.cn

Ruby: warn "err"
来源：http://tqr.xuanzx.com

C#:   Console.Error.WriteLine("err")
来源：http://ylr.zdbjq.cn

[M07] 判断是否为主入口
来源：http://pgy.daxiang520.top

Py:   if __name__ == "__main__":
来源：http://qxx.havefunace.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bvz.bjfxy.top

JS:   require.main === module
来源：http://ipr.nanxinkj.top

TS:   require.main === module
来源：http://wki.kuanghao11.cn

Java: public static void main(String[] args)
来源：http://wgc.chenzaomai.com

Go:   func main()
来源：http://vqq.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://psw.gotoacloud.top

C#:   static void Main(string[] args)
来源：http://bjf.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://ooo.tian-w.cn

Py:   platform.system();  platform.python_version()
来源：http://ejr.zhengqikj.top

PHP:  PHP_OS;  phpversion();
来源：http://uqu.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://tba.shuidangran.top

TS:   process.platform;  process.version
来源：http://xuz.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://adr.svipenyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ude.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yed.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://tbz.cashguo.top

================================================================================
来源：http://rpr.fehbvm.com

N. 数据结构与算法
来源：http://kvn.vehdjk.com

================================================================================
来源：http://cfb.dianchejie.cn

[N01] 二分查找（有序数组）
来源：http://mua.xinyue.icu

Py:   bisect.bisect_left(arr, x)
来源：http://jvz.jlsjyb.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bwe.ctjpmb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lpq.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sdl.ybcxt.top

Java: Arrays.binarySearch(arr, x)
来源：http://dif.gogol.net.cn

Go:   sort.SearchInts(arr, x)
来源：http://dls.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://lbu.zdbjq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cbs.daxiang520.top

[N02] 排序（工程实践用内置实现）
来源：http://sfb.nwbrower.top

Py:   sorted(arr);  arr.sort()
来源：http://pvj.jyoumei.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qpk.jqgfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://dot.shanyushiyangtech.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dur.guowangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://thh.fehbvm.com

Go:   slices.Sort(arr)
来源：http://sxh.hfpthk.cn

Ruby: arr.sort
来源：http://fnq.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://mnl.hnxiangtu.top

[N03] 快速排序（分治示例）
来源：http://rku.tianlin.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lbb.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://dxs.hnqzz.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cem.jinqigufen.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jzs.jqgufenzy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vxm.fanxiaobao.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sfe.gzhubu.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://evy.vqdsnc.cn

C#:   // 手写递归，或 Array.Sort
来源：http://tnt.nanxuanxn.top

[N04] 斐波那契数列
来源：http://kwk.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zgz.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vnq.guowangkeji.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://niy.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dfu.daxiang520.top


<!-- 参考信息 -->