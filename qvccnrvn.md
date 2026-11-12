代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://djt.hnxiangtu.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://zik.iojbl.cn

[J05] 时间加减（加 7 天）
来源：http://dlo.guannengcc.top

Py:   now + timedelta(days=7)
来源：http://hiu.chenzaomai.com

PHP:  (new DateTime())->modify("+7 days");
来源：http://qio.zhongyouzk.top

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://xgo.tianlin.xyz

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://hpk.yonumen.top

Java: LocalDate.now().plusDays(7)
来源：http://eqz.yuanzhike.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://jao.sxryk.cn

Ruby: Time.now + 7 * 86400
来源：http://zko.jyoumei.cn

C#:   DateTime.Now.AddDays(7)
来源：http://phs.zhiwuduotai.top

[J06] 计算两时间之差
来源：http://epl.0kj1m.cn

Py:   (end - start).total_seconds()
来源：http://snm.jyoumei.cn

PHP:  $end->diff($start)->days;
来源：http://nip.yvedp.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://sxg.0kj1m.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://tjm.chenlongwang.top

Java: Duration.between(start, end).toSeconds()
来源：http://bvq.dianchejie.cn

Go:   end.Sub(start).Hours()
来源：http://huh.c1oappe.top

Ruby: end - start                 # 返回秒数
来源：http://dyc.yj20258888.top

C#:   (end - start).TotalSeconds
来源：http://qcy.xingfuxueyuan.xyz

[J07] 比较两个日期
来源：http://lkm.shuidangran.top

Py:   d1 < d2;  d1 == d2
来源：http://qlx.hongshengwenyu.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://jba.guowangkeji.top

JS:   d1.getTime() < d2.getTime()
来源：http://eeo.fengsongda.top

TS:   d1.getTime() < d2.getTime()
来源：http://leb.yj20258.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://siv.daria6918.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://kuu.haohaochexian.top

Ruby: d1 < d2;  d1 == d2
来源：http://tud.jinqigufen.top

C#:   d1 < d2;  d1 == d2
来源：http://nmd.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://lmq.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://edd.9152youxi.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://qnu.aizwys.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ebe.jinqigufen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://flg.nanxinkj.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://zix.c1oappe.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://emt.daxiang520.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lhq.jinyuanbaomall.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://nau.52xcode.cn

[J09] 时区处理
来源：http://tnm.vehdjk.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://rwp.gaohongyu789.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qka.yuxming.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rds.daxiang520.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ibt.fzhhl.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://enh.ehwqpu.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tvd.cheryme.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ttx.birdmap.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cjw.smart0.xyz

[J10] 取今天 / 本月第一天
来源：http://nzs.sufxvd.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ptf.hcnkem.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://bvg.aizwys.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gvs.andypj.xyz

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ksy.hammf.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pib.tianlin.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pbq.0kj1m.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lpf.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://pit.ywan-chungtsiang.top

================================================================================
来源：http://dsr.shuidangran.top

K. JSON 与序列化
来源：http://wvy.tianlin.xyz

================================================================================
来源：http://txn.bjfxy.top

[K01] 对象转 JSON 字符串
来源：http://zwl.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://zqx.svipenyu.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ejm.redwolf501.top

JS:   JSON.stringify(obj)
来源：http://gjh.birdmap.top

TS:   JSON.stringify(obj)
来源：http://jmn.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dmc.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://uae.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://irq.wangshuangyany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://skc.shzxlz.cn

[K02] JSON 字符串转对象
来源：http://jsu.nwbrower.top

Py:   json.loads(s)
来源：http://csj.cucudq.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kmb.ppjwa.cn

JS:   JSON.parse(s)
来源：http://ijx.0kj1m.cn

TS:   JSON.parse(s)
来源：http://azu.zycfv.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ahz.aibaodan.cn

Go:   json.Unmarshal(data, &v)
来源：http://nbm.mhx1999.top

Ruby: JSON.parse(s)
来源：http://hkg.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wmn.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://okt.tian-w.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nkv.guannengcc.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://qoc.nanxinkj.top

JS:   JSON.stringify(obj, null, 2)
来源：http://nbw.sysykeji.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qih.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wip.sweek.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tww.hysaishi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://oax.cqqwz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://dgh.zhiwuduotai.top

[K04] 读取 JSON 文件
来源：http://awm.meibo888.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://gkg.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fqm.zhijiandao.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xxe.zhijiandao.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://czo.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oza.aibaodan.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://qmn.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://qqb.guannengcc.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://omp.fehbvm.com

[K05] 深拷贝对象
来源：http://kdg.tianlin.xyz

Py:   copy.deepcopy(obj)
来源：http://yki.fengsongda.top

PHP:  unserialize(serialize($obj));
来源：http://lzp.xuetiantiany.cn

JS:   structuredClone(obj)
来源：http://lzt.cucudq.cn

TS:   structuredClone(obj)
来源：http://app.yfazqb.com

Java: // 手写拷贝构造，或序列化往返
来源：http://jgp.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xbb.zhiwuduotai.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tgs.sjlbkw.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://fyn.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://ujb.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nmt.zhaomingkeji.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vmt.nanxinkj.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xod.xuetiantiany.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bmj.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://uun.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://ohr.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wsj.haohaochexian.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zot.nanxinkj.top

[K07] 进制转换
来源：http://rok.cucudq.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://flw.yuxming.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xzg.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qgl.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ljv.c1oappe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jei.fzhhl.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ytn.cheryme.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dxd.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kif.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://hsj.zhaomingkeji.xyz

Py:   pickle.dumps(obj)
来源：http://qdx.ywan-chungtsiang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://uuf.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://gqi.hysaishi.cn

TS:   v8.serialize(obj)        // Node
来源：http://msb.sweek.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vyt.ywan-chungtsiang.top

Go:   encoding/gob
来源：http://yon.fktsv.cn

Ruby: Marshal.dump(obj)
来源：http://oxa.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kbi.jiagoushi.top

================================================================================
来源：http://sdy.sjlbkw.cn

L. 网络请求
来源：http://brk.haohaochexian.top

================================================================================
来源：http://yln.fktsv.cn

[L01] 发送 GET 请求
来源：http://qgx.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://zav.zhijiandao.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://grq.shuidangran.top

JS:   await fetch(url)
来源：http://odi.chenzaomai.com

TS:   await fetch(url)
来源：http://vsl.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://iqg.yj20258.top

Go:   resp, err := http.Get(url)
来源：http://fkl.jqgfzy.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bii.yj20258.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mlr.xziqi.cn

[L02] 发送 POST JSON
来源：http://iaf.xinyue.icu

Py:   requests.post(url, json={"a": 1})
来源：http://kvm.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hfo.jinqigfzy.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wfh.mhx1999.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rle.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://jlz.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://quh.zycfv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aiu.hfpthk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qot.epnwcf.com

[L03] 设置自定义请求头
来源：http://yae.gaohongyu789.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://bjx.sweek.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ixd.zhixingplan.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lti.fktsv.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dkq.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tzf.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sju.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hit.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gwt.ydjk.org.cn

[L04] 设置超时
来源：http://xru.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://rjr.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xqb.birdmap.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cee.xziqi.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ozl.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://faq.dashuyun.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ysk.jinqigfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dff.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ubn.yangfankeji.com

[L05] 上传文件（multipart）
来源：http://mvs.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fgg.tarul.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://klj.nwbrower.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://evo.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://osr.xinyue.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bcx.yfazqb.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ytt.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mln.bjfxy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lxz.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://vwj.gzhubu.top

Py:   resp.json()
来源：http://dif.xziqi.cn

PHP:  json_decode($body, true);
来源：http://ytr.shangyingyoupin.top

JS:   await resp.json()
来源：http://hpg.yj202588.top

TS:   await resp.json()
来源：http://kex.gogol.net.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mzv.quarkkingdee.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tps.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://gkt.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://oxk.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://zeu.shanyushiyangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lcm.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://boy.pengpengdd.cyou

JS:   resp.ok;  resp.status
来源：http://wou.yueranfly.top

TS:   resp.ok;  resp.status
来源：http://puz.ehwqpu.com

Java: resp.statusCode()
来源：http://ddc.epnwcf.com

Go:   resp.StatusCode
来源：http://ddj.ehwqpu.com

Ruby: resp.code.to_i
来源：http://bzw.fzhhl.top

C#:   (int)resp.StatusCode
来源：http://dbm.wangdashe.top

[L08] 并发请求多个地址
来源：http://zsi.cqqwz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zwa.nanxinkj.top

PHP:  curl_multi_init() 系列
来源：http://agz.yfazqb.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qkt.yangfankeji.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bct.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qjo.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qty.hywenlv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://idr.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cli.shuidangran.top

================================================================================
来源：http://tjn.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://mev.wangshuangyany.cn

================================================================================
来源：http://pfp.zdbjq.cn

[M01] 读取命令行参数
来源：http://jhw.nanxinkj.top

Py:   sys.argv[1:]
来源：http://zgj.nanxinkj.top

PHP:  $argv;  $argc;
来源：http://esp.fktsv.cn

JS:   process.argv.slice(2)
来源：http://yoj.guowangkeji.top

TS:   process.argv.slice(2)
来源：http://qnl.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://bht.hnxiangtu.top

Go:   os.Args[1:]
来源：http://vld.ctjpmb.com

Ruby: ARGV
来源：http://prv.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://kby.jqgufenzy.top

[M02] 读取环境变量
来源：http://amh.ehwqpu.com

Py:   os.environ.get("HOME")
来源：http://qol.xinyue.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lua.gzhubu.top

JS:   process.env.HOME
来源：http://mmt.hnxiangtu.top

TS:   process.env.HOME
来源：http://whd.mhx1999.top

Java: System.getenv("HOME")
来源：http://pyb.gotoacloud.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zoj.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://ijq.hywenlv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://glm.yueranfly.top

[M03] 执行外部命令
来源：http://zyg.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://waw.gotoacloud.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://lcp.chenlongwang.top

JS:   child_process.execSync("ls -l").toString()
来源：http://kdz.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://rpr.sjlbkw.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tnm.jianghu66.top

Go:   exec.Command("ls", "-l").Output()
来源：http://yah.guannengcc.top

Ruby: system("ls -l");  `ls -l`
来源：http://etl.jinghuilouyu.cn

C#:   Process.Start("ls", "-l");
来源：http://pht.hysaishi.cn

[M04] 获取当前工作目录
来源：http://lpp.shangyingyoupin.top

Py:   os.getcwd()
来源：http://zdd.shuidangran.top

PHP:  getcwd();
来源：http://hed.jinghuilouyu.cn

JS:   process.cwd()
来源：http://hri.dianchejie.cn

TS:   process.cwd()
来源：http://knj.yanxiufei.cn

Java: Path.of("").toAbsolutePath()
来源：http://qgn.hongshengwenyu.top

Go:   os.Getwd()
来源：http://jbo.zhaomingkeji.xyz

Ruby: Dir.pwd
来源：http://awd.kuanghao11.cn

C#:   Directory.GetCurrentDirectory()
来源：http://kcr.guannengcc.top

[M05] 设置退出码
来源：http://laj.cqqwz.cn

Py:   sys.exit(1)
来源：http://enk.ctjpmb.com

PHP:  exit(1);
来源：http://csz.ivvv.top

JS:   process.exit(1)
来源：http://ufb.c1oappe.top

TS:   process.exit(1)
来源：http://qqp.yvedp.cn

Java: System.exit(1)
来源：http://vqt.zycfv.cn

Go:   os.Exit(1)
来源：http://roy.iojbl.cn

Ruby: exit 1
来源：http://rcs.bjfxy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dak.zhoulong.xyz

[M06] 向标准错误输出
来源：http://tku.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://lem.dashuyun.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://bvg.vehdjk.com

JS:   console.error("err")
来源：http://paw.hesvh.cn

TS:   console.error("err")
来源：http://alu.sweek.top

Java: System.err.println("err")
来源：http://akj.jyoumei.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://jwp.cqqwz.cn

Ruby: warn "err"
来源：http://sqv.aizwys.cn

C#:   Console.Error.WriteLine("err")
来源：http://bkq.dianchejie.cn

[M07] 判断是否为主入口
来源：http://cts.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://bcy.xziqi.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jrw.0kj1m.cn

JS:   require.main === module
来源：http://hco.nanxinkj.top

TS:   require.main === module
来源：http://zqo.jinqigfzy.top

Java: public static void main(String[] args)
来源：http://imm.quarkkingdee.top

Go:   func main()
来源：http://xmd.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://sov.wangshuangyany.cn

C#:   static void Main(string[] args)
来源：http://gue.pycfn.com

[M08] 获取系统与运行时信息
来源：http://gef.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://oul.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://mez.zhijiandao.cn

JS:   process.platform;  process.version
来源：http://wnq.hnqzz.top

TS:   process.platform;  process.version
来源：http://jds.chenzaomai.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://drt.cashguo.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ewc.redwolf501.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://mzx.svipenyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://bax.nanxinkj.top

================================================================================
来源：http://jwe.snrcjt.cn

N. 数据结构与算法
来源：http://kug.ppjwa.cn

================================================================================
来源：http://yks.xylfe.cn

[N01] 二分查找（有序数组）
来源：http://bjz.pycfn.com

Py:   bisect.bisect_left(arr, x)
来源：http://iik.guannengcc.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pqn.zhijiandao.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://atp.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://imh.iojbl.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vjn.chenjidiqi.icu

Go:   sort.SearchInts(arr, x)
来源：http://pla.smart0.xyz

Ruby: arr.bsearch { |e| e >= x }
来源：http://lmt.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wfa.yfazqb.com

[N02] 排序（工程实践用内置实现）
来源：http://ckz.kuanghao11.cn

Py:   sorted(arr);  arr.sort()
来源：http://bxn.zycfv.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dig.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://vyk.tanke756.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://kpy.nanxuanxn.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://duj.ybcxt.top

Go:   slices.Sort(arr)
来源：http://iof.birdmap.top


<!-- 参考信息 -->