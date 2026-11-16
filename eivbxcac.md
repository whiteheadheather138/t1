代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://owx.yfazqb.com

Ruby: Time.now + 7 * 86400
来源：http://phk.ydzc1.top

C#:   DateTime.Now.AddDays(7)
来源：http://tso.chenlongwang.top

[J06] 计算两时间之差
来源：http://pro.jlsjyb.cn

Py:   (end - start).total_seconds()
来源：http://psb.gaohongyu789.top

PHP:  $end->diff($start)->days;
来源：http://phd.yfazqb.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://uhg.fanxiaobao.xyz

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://bet.aizwys.cn

Java: Duration.between(start, end).toSeconds()
来源：http://byh.gotoacloud.top

Go:   end.Sub(start).Hours()
来源：http://sxr.birdmap.top

Ruby: end - start                 # 返回秒数
来源：http://mdv.nanxinkj.top

C#:   (end - start).TotalSeconds
来源：http://rga.zycfv.cn

[J07] 比较两个日期
来源：http://dkg.xziqi.cn

Py:   d1 < d2;  d1 == d2
来源：http://jgb.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://djd.dianchejie.cn

JS:   d1.getTime() < d2.getTime()
来源：http://odh.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://bro.shuidangran.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ysw.svipenyu.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kbl.hnxiangtu.top

Ruby: d1 < d2;  d1 == d2
来源：http://ecp.andypj.xyz

C#:   d1 < d2;  d1 == d2
来源：http://llo.yongpay.top

[J08] 提取年月日与星期
来源：http://vag.fehbvm.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://wjy.aibaodan.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lmn.shuidangran.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xki.jinqigfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://nse.9152youxi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://gyw.yongpay.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ych.vqdsnc.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hun.yanxiufei.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://vxl.ehwqpu.com

[J09] 时区处理
来源：http://yul.ppjwa.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://cou.quarkkingdee.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xpa.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hbv.ybcxt.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://puw.zycfv.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://pda.316326.xyz

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://eks.guannengcc.top

Ruby: Time.now.getlocal("+08:00")
来源：http://efd.xziqi.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://evs.chenjidiqi.icu

[J10] 取今天 / 本月第一天
来源：http://aud.zhoulong.xyz

Py:   date.today();  date.today().replace(day=1)
来源：http://njl.52xcode.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fhu.jqgfzy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://uvt.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jek.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jgn.yuxming.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zmn.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://iqp.chenlongwang.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://asz.316326.xyz

================================================================================
来源：http://ecn.zycfv.cn

K. JSON 与序列化
来源：http://zmk.birdmap.top

================================================================================
来源：http://uex.zdbjq.cn

[K01] 对象转 JSON 字符串
来源：http://wod.cqqwz.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://znq.ctjpmb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jxj.9152youxi.cn

JS:   JSON.stringify(obj)
来源：http://fub.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://yuf.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nwj.shanyushiyangkeji.top

Go:   json.Marshal(obj)
来源：http://oxc.jyoumei.cn

Ruby: obj.to_json                                     // require "json"
来源：http://nod.iojbl.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jek.yonumen.top

[K02] JSON 字符串转对象
来源：http://wcb.jiagoushi.top

Py:   json.loads(s)
来源：http://fmq.316326.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://aed.tian-w.cn

JS:   JSON.parse(s)
来源：http://iaj.quarkkingdee.top

TS:   JSON.parse(s)
来源：http://zwx.hnxiangtu.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vho.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://bna.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://xgq.cashguo.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sji.ehwqpu.com

[K03] JSON 美化输出（带缩进）
来源：http://hld.zhiwuduotai.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://prp.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vdk.kuanghao11.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://oty.shuidangran.top

TS:   JSON.stringify(obj, null, 2)
来源：http://kln.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zwb.xylfe.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sbm.kuanghao11.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nug.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qyj.zhaomingkeji.xyz

[K04] 读取 JSON 文件
来源：http://ras.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://leb.fzhhl.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://icg.xziqi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fbj.tanke756.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xlw.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mkz.xziqi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ego.c1oappe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://onz.aizwys.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fqg.yonumen.top

[K05] 深拷贝对象
来源：http://mgx.gotoacloud.top

Py:   copy.deepcopy(obj)
来源：http://vpl.chenjidiqi.icu

PHP:  unserialize(serialize($obj));
来源：http://kzf.zhixingplan.top

JS:   structuredClone(obj)
来源：http://jlr.dashuyun.cn

TS:   structuredClone(obj)
来源：http://euj.hysaishi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://wwn.316326.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ifg.ehwqpu.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cui.tanke756.top

C#:   // 序列化往返，或自定义 Clone
来源：http://oxh.gotoacloud.top

[K06] 解析 URL 查询串
来源：http://mbc.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ofe.mhx1999.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ilr.sxryk.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://auh.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://tsd.zhongyouzk.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://stt.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tla.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://suc.cucudq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hgq.ybcxt.top

[K07] 进制转换
来源：http://rko.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tku.hcnkem.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gni.meibo888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ewf.fzhhl.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hzy.daxiang520.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://uaw.yongpay.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://atl.chenjidiqi.icu

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://llu.wangshuangyany.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ocy.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://qgf.yongpay.top

Py:   pickle.dumps(obj)
来源：http://qsf.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://igy.jiagoushi.top

JS:   v8.serialize(obj)        // Node
来源：http://rxs.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ntp.yonumen.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://qxb.tianlin.xyz

Go:   encoding/gob
来源：http://xue.vqdsnc.cn

Ruby: Marshal.dump(obj)
来源：http://yjh.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sny.jinyuanbaomall.cn

================================================================================
来源：http://qfn.sjlbkw.cn

L. 网络请求
来源：http://bws.ivvv.top

================================================================================
来源：http://qix.aibaodan.cn

[L01] 发送 GET 请求
来源：http://vsq.zdbjq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yvt.aizwys.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ufc.bjfxy.top

JS:   await fetch(url)
来源：http://kas.xylfe.cn

TS:   await fetch(url)
来源：http://kam.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tpp.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://hjx.shanyushiyangtech.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qxk.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ujj.chenzaomai.com

[L02] 发送 POST JSON
来源：http://aus.zycfv.cn

Py:   requests.post(url, json={"a": 1})
来源：http://lia.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wxu.aizwys.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kwg.andypj.xyz

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lto.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://rqe.aizwys.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xwf.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ckp.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gfu.zhixingplan.top

[L03] 设置自定义请求头
来源：http://qjz.yonumen.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://cuv.0kj1m.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aiu.gzhubu.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ewx.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fcb.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yur.yuanzhike.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uzf.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dis.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eje.vehdjk.com

[L04] 设置超时
来源：http://irp.cqqwz.cn

Py:   requests.get(url, timeout=5)
来源：http://pxz.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://kzk.aizwys.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bra.daria6918.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wjn.hnxiangtu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qwx.haohaochexian.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://snn.havefunace.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pht.jlsjyb.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://npz.yuxming.cn

[L05] 上传文件（multipart）
来源：http://tbq.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://koi.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uzl.zhixingplan.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vhm.ppjwa.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pnr.xziqi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zof.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://twd.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ehs.tarul.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dwm.yj20258888.top

[L06] 解析响应为 JSON
来源：http://zbx.pengpengdd.cyou

Py:   resp.json()
来源：http://rto.pycfn.com

PHP:  json_decode($body, true);
来源：http://mfd.havefunace.top

JS:   await resp.json()
来源：http://ide.yj20258888.top

TS:   await resp.json()
来源：http://req.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xdw.vqdsnc.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kaq.daxiang520.top

Ruby: JSON.parse(resp.body)
来源：http://bzw.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rmf.yuxming.cn

[L07] 处理 HTTP 状态码
来源：http://abe.haohaochexian.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://fzk.epnwcf.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ujd.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://tcf.xylfe.cn

TS:   resp.ok;  resp.status
来源：http://atv.ivvv.top

Java: resp.statusCode()
来源：http://gux.epnwcf.com

Go:   resp.StatusCode
来源：http://yvk.dianchejie.cn

Ruby: resp.code.to_i
来源：http://eex.yj202588.top

C#:   (int)resp.StatusCode
来源：http://osw.316326.xyz

[L08] 并发请求多个地址
来源：http://hbb.ydjk.org.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://khe.chenlongwang.top

PHP:  curl_multi_init() 系列
来源：http://vrr.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://srs.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qcx.hcnkem.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://msz.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lbm.pycfn.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://pox.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://skr.nwbrower.top

================================================================================
来源：http://fnu.zhengqikj.top

M. 命令行 / 进程 / 环境
来源：http://eex.sjlbkw.cn

================================================================================
来源：http://ksj.dianchejie.cn

[M01] 读取命令行参数
来源：http://drt.fengsongda.top

Py:   sys.argv[1:]
来源：http://ohd.wangdashe.top

PHP:  $argv;  $argc;
来源：http://qbu.yongpay.top

JS:   process.argv.slice(2)
来源：http://lal.xuetiantiany.cn

TS:   process.argv.slice(2)
来源：http://bmn.daxiang520.top

Java: args 数组（main 方法参数）
来源：http://qbw.cucudq.cn

Go:   os.Args[1:]
来源：http://tte.hammf.cn

Ruby: ARGV
来源：http://uim.shzxlz.cn

C#:   args 数组（Main 方法参数）
来源：http://wrm.ppjwa.cn

[M02] 读取环境变量
来源：http://amf.xuanzx.com

Py:   os.environ.get("HOME")
来源：http://uxi.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://voq.jyoumei.cn

JS:   process.env.HOME
来源：http://yfd.chenlongwang.top

TS:   process.env.HOME
来源：http://mpb.yonumen.top

Java: System.getenv("HOME")
来源：http://sdi.shangyingyoupin.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dmn.mhx1999.top

Ruby: ENV["HOME"]
来源：http://jfh.aibaodan.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bgd.gzhubu.top

[M03] 执行外部命令
来源：http://eqq.kuanghao11.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vpf.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zrh.cucudq.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zrj.xinyue.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://iyh.sysykeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ijd.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wkd.kuanghao11.cn

Ruby: system("ls -l");  `ls -l`
来源：http://ceq.cucudq.cn

C#:   Process.Start("ls", "-l");
来源：http://mwa.guannengcc.top

[M04] 获取当前工作目录
来源：http://iek.fengsongda.top

Py:   os.getcwd()
来源：http://tpy.hongshengwenyu.top

PHP:  getcwd();
来源：http://ndu.chenlongwang.top

JS:   process.cwd()
来源：http://frq.yongpay.top

TS:   process.cwd()
来源：http://xko.tanke756.top

Java: Path.of("").toAbsolutePath()
来源：http://slk.zdbjq.cn

Go:   os.Getwd()
来源：http://ikr.nanxuanxn.top

Ruby: Dir.pwd
来源：http://lid.fengsongda.top

C#:   Directory.GetCurrentDirectory()
来源：http://oxb.jqgfzy.top

[M05] 设置退出码
来源：http://qoh.meibo888.top

Py:   sys.exit(1)
来源：http://trs.yj20258.top

PHP:  exit(1);
来源：http://yrc.zycfv.cn

JS:   process.exit(1)
来源：http://crv.jyoumei.cn

TS:   process.exit(1)
来源：http://nuh.pycfn.com

Java: System.exit(1)
来源：http://ogm.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://kra.redwolf501.top

Ruby: exit 1
来源：http://jbx.yuxming.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tkg.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://bfs.zhaomingkeji.xyz

Py:   print("err", file=sys.stderr)
来源：http://stx.jianghu66.top

PHP:  fwrite(STDERR, "err\n");
来源：http://wjk.mhx1999.top

JS:   console.error("err")
来源：http://wts.hnxiangtu.top

TS:   console.error("err")
来源：http://wun.hnxiangtu.top

Java: System.err.println("err")
来源：http://sii.pycfn.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mal.tianlin.xyz

Ruby: warn "err"
来源：http://cnz.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://sjj.aizwys.cn

[M07] 判断是否为主入口
来源：http://uso.xziqi.cn

Py:   if __name__ == "__main__":
来源：http://trg.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kbx.xylfe.cn

JS:   require.main === module
来源：http://udp.cucudq.cn

TS:   require.main === module
来源：http://twk.xingfuxueyuan.xyz

Java: public static void main(String[] args)
来源：http://nip.gotoacloud.top

Go:   func main()
来源：http://ism.zhengqikj.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://kzc.bbcook.cn

C#:   static void Main(string[] args)
来源：http://ijo.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://fmt.c1oappe.top

Py:   platform.system();  platform.python_version()
来源：http://lij.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://ora.xingfuxueyuan.xyz

JS:   process.platform;  process.version
来源：http://aoa.guannengcc.top

TS:   process.platform;  process.version
来源：http://cjr.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://tsw.uphjek.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://xda.haohaochexian.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ozs.vehdjk.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://qmq.zdbjq.cn

================================================================================
来源：http://bql.jinqigfzy.top

N. 数据结构与算法
来源：http://eyg.wangdashe.top

================================================================================
来源：http://mmf.shzxlz.cn

[N01] 二分查找（有序数组）
来源：http://tel.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://prt.sweek.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vyr.wangdashe.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://auv.hnxiangtu.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ruq.jiagoushi.top

Java: Arrays.binarySearch(arr, x)
来源：http://qwc.cdnleiting.top

Go:   sort.SearchInts(arr, x)
来源：http://zjm.feifeiyinyue.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rtn.redwolf501.top

C#:   Array.BinarySearch(arr, x)
来源：http://mwv.guannengcc.top

[N02] 排序（工程实践用内置实现）
来源：http://ccu.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://lqu.svipenyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ibq.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ixs.nanxinkj.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://zyq.shanyushiyangkeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://oyv.316326.xyz

Go:   slices.Sort(arr)
来源：http://wni.daria6918.cn

Ruby: arr.sort
来源：http://wid.cashguo.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://kfb.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://dpb.sweek.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wpl.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://inr.zhijiandao.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ukb.bjfxy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yza.dashuyun.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nvs.shzxlz.cn


<!-- 参考信息 -->