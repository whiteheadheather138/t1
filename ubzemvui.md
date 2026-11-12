代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://bcr.daria6918.cn

Ruby: Time.now + 7 * 86400
来源：http://utu.gotoacloud.top

C#:   DateTime.Now.AddDays(7)
来源：http://goa.aibaodan.cn

[J06] 计算两时间之差
来源：http://bcz.yuxming.cn

Py:   (end - start).total_seconds()
来源：http://qmf.zhixingplan.top

PHP:  $end->diff($start)->days;
来源：http://qii.sxryk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://mjt.ppjwa.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kpr.aizwys.cn

Java: Duration.between(start, end).toSeconds()
来源：http://dzv.hesvh.cn

Go:   end.Sub(start).Hours()
来源：http://kve.tarul.cn

Ruby: end - start                 # 返回秒数
来源：http://izp.yangfankeji.com

C#:   (end - start).TotalSeconds
来源：http://srb.pycfn.com

[J07] 比较两个日期
来源：http://sft.sjlbkw.cn

Py:   d1 < d2;  d1 == d2
来源：http://zsq.ydzc1.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://ded.jinqigfzy.top

JS:   d1.getTime() < d2.getTime()
来源：http://wqe.cqqwz.cn

TS:   d1.getTime() < d2.getTime()
来源：http://atw.hongshengwenyu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qzj.tianlin.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vha.daxiang520.top

Ruby: d1 < d2;  d1 == d2
来源：http://cqy.tanke756.top

C#:   d1 < d2;  d1 == d2
来源：http://wem.jiagoushi.top

[J08] 提取年月日与星期
来源：http://tpq.zhiwuduotai.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://usa.cqqwz.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zxd.bbcook.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://zxv.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://shd.tianlin.xyz

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bwo.nanxinkj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fnc.bjfxy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://way.guannengcc.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ojh.yanxiufei.cn

[J09] 时区处理
来源：http://sxf.quarkkingdee.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://roc.ppjwa.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://shb.tarul.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://oen.vehdjk.com

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jzb.jiagoushi.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://cbj.ybcxt.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://bev.9152youxi.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://xiu.bbcook.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jag.aizwys.cn

[J10] 取今天 / 本月第一天
来源：http://xlc.chenzaomai.com

Py:   date.today();  date.today().replace(day=1)
来源：http://ulo.cqqwz.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vgk.vehdjk.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qrl.yj202588.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pnm.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gpe.xuanzx.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yyp.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rhl.meibo888.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://daq.zdqjudy.top

================================================================================
来源：http://myt.sufxvd.cn

K. JSON 与序列化
来源：http://epd.ivvv.top

================================================================================
来源：http://rgd.feifeiyinyue.top

[K01] 对象转 JSON 字符串
来源：http://nli.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ejs.kuanghao11.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qas.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://nwe.gzhubu.top

TS:   JSON.stringify(obj)
来源：http://eoq.yongpay.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://efn.fzhhl.top

Go:   json.Marshal(obj)
来源：http://jwr.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://hvf.wangdashe.top

C#:   JsonSerializer.Serialize(obj)
来源：http://uxs.guowangkeji.top

[K02] JSON 字符串转对象
来源：http://pkm.fzhhl.top

Py:   json.loads(s)
来源：http://ktj.ydjk.org.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qdo.zhaomingkeji.xyz

JS:   JSON.parse(s)
来源：http://wob.zhaomingkeji.xyz

TS:   JSON.parse(s)
来源：http://xng.feifeiyinyue.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nzl.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://vit.fehbvm.com

Ruby: JSON.parse(s)
来源：http://vwo.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://vlz.sweek.top

[K03] JSON 美化输出（带缩进）
来源：http://taw.ybcxt.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gar.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://mvp.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qpv.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qlp.hammf.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sdg.tarul.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://beg.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://usw.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jyl.316326.xyz

[K04] 读取 JSON 文件
来源：http://hwk.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pxo.snrcjt.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wdz.sysykeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://joc.jinqigfzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zaj.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rwa.xingfuxueyuan.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://tyi.cheryme.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://icm.zhoulong.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://pim.0kj1m.cn

[K05] 深拷贝对象
来源：http://nux.jinyuanbaomall.cn

Py:   copy.deepcopy(obj)
来源：http://bbh.gogol.net.cn

PHP:  unserialize(serialize($obj));
来源：http://meh.shzxlz.cn

JS:   structuredClone(obj)
来源：http://zbu.ppjwa.cn

TS:   structuredClone(obj)
来源：http://xtz.shzxlz.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://hir.kuanghao11.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eal.sufxvd.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zbw.ppjwa.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ihp.cashguo.top

[K06] 解析 URL 查询串
来源：http://rmn.guowangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://tfv.gzhubu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://swd.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vgd.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cxx.yuanzhike.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vtu.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://bkc.yueranfly.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nog.yfazqb.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dju.fanxiaobao.xyz

[K07] 进制转换
来源：http://kwf.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hjg.hywenlv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://grq.gzhubu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://tft.cashguo.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uyi.shangyingyoupin.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://cwt.sysykeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ufq.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uyw.nanxuanxn.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://pkx.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://xvg.vqdsnc.cn

Py:   pickle.dumps(obj)
来源：http://dge.dianchejie.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nol.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://cie.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://cym.ppjwa.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ajd.smart0.xyz

Go:   encoding/gob
来源：http://csq.cheryme.top

Ruby: Marshal.dump(obj)
来源：http://knm.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xwp.wangshuangyany.cn

================================================================================
来源：http://fsx.jinghuilouyu.cn

L. 网络请求
来源：http://hrd.nanxinkj.top

================================================================================
来源：http://ebs.aibaodan.cn

[L01] 发送 GET 请求
来源：http://bfh.sysykeji.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://urq.mhx1999.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tte.yangfankeji.com

JS:   await fetch(url)
来源：http://ouq.shangyingyoupin.top

TS:   await fetch(url)
来源：http://vov.smart0.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tsi.hammf.cn

Go:   resp, err := http.Get(url)
来源：http://qts.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://yho.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tkk.zhixingplan.top

[L02] 发送 POST JSON
来源：http://pko.vqdsnc.cn

Py:   requests.post(url, json={"a": 1})
来源：http://skx.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jrb.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rqv.tanke756.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mds.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hgf.fzhhl.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://orp.ehwqpu.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ipy.uphjek.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nfr.bjfxy.top

[L03] 设置自定义请求头
来源：http://tko.birdmap.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gyw.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://eaj.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pcb.gotoacloud.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wzn.yj20258.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tsk.hnqzz.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://vfq.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ugw.zhongyouzk.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dim.bbcook.cn

[L04] 设置超时
来源：http://wla.tianlin.xyz

Py:   requests.get(url, timeout=5)
来源：http://byx.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mrg.hammf.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vce.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://des.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jws.zdqjudy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aeq.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://lwu.epnwcf.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zlp.nanxuanxn.top

[L05] 上传文件（multipart）
来源：http://aen.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lmh.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rbz.jyoumei.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jya.aibaodan.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wav.nwbrower.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://tky.quarkkingdee.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mps.zycfv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pov.xuanzx.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://myz.hysaishi.cn

[L06] 解析响应为 JSON
来源：http://oku.shuidangran.top

Py:   resp.json()
来源：http://vwu.sysykeji.top

PHP:  json_decode($body, true);
来源：http://pud.uphjek.com

JS:   await resp.json()
来源：http://vbn.epnwcf.com

TS:   await resp.json()
来源：http://sak.aibaodan.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xud.tian-w.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wgy.zdbjq.cn

Ruby: JSON.parse(resp.body)
来源：http://icp.feifeiyinyue.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rvd.pycfn.com

[L07] 处理 HTTP 状态码
来源：http://uoe.tarul.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vhk.cashguo.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hch.shanyushiyangtech.top

JS:   resp.ok;  resp.status
来源：http://aao.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://zdf.jlsjyb.cn

Java: resp.statusCode()
来源：http://lnp.sysykeji.top

Go:   resp.StatusCode
来源：http://ifl.dashuyun.cn

Ruby: resp.code.to_i
来源：http://vpm.shangyingyoupin.top

C#:   (int)resp.StatusCode
来源：http://nna.guannengcc.top

[L08] 并发请求多个地址
来源：http://uar.hnqzz.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://evc.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://kej.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://wym.c1oappe.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ckk.hesvh.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ytn.yueranfly.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zhg.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://plu.xinyue.icu

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ljw.yj20258.top

================================================================================
来源：http://fjo.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://rgk.dashuyun.cn

================================================================================
来源：http://rad.hcnkem.com

[M01] 读取命令行参数
来源：http://omc.gotoacloud.top

Py:   sys.argv[1:]
来源：http://nsy.iojbl.cn

PHP:  $argv;  $argc;
来源：http://lgw.zhoulong.xyz

JS:   process.argv.slice(2)
来源：http://qkq.316326.xyz

TS:   process.argv.slice(2)
来源：http://blt.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://xgi.sweek.top

Go:   os.Args[1:]
来源：http://wae.316326.xyz

Ruby: ARGV
来源：http://yat.shanyushiyangkeji.top

C#:   args 数组（Main 方法参数）
来源：http://nei.zhixingplan.top

[M02] 读取环境变量
来源：http://adt.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://duh.feifeiyinyue.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://iyk.gaohongyu789.top

JS:   process.env.HOME
来源：http://ahx.birdmap.top

TS:   process.env.HOME
来源：http://qzi.pengpengdd.cyou

Java: System.getenv("HOME")
来源：http://jvt.hysaishi.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zad.ctjpmb.com

Ruby: ENV["HOME"]
来源：http://wuq.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://krv.snrcjt.cn

[M03] 执行外部命令
来源：http://epl.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hyw.jianghu66.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://poi.daria6918.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xai.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://vep.bjfxy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cks.zhixingplan.top

Go:   exec.Command("ls", "-l").Output()
来源：http://exk.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xcl.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://ard.cqqwz.cn

[M04] 获取当前工作目录
来源：http://lha.shanyushiyangtech.top

Py:   os.getcwd()
来源：http://woe.iojbl.cn

PHP:  getcwd();
来源：http://uem.xziqi.cn

JS:   process.cwd()
来源：http://ayl.ppjwa.cn

TS:   process.cwd()
来源：http://mbd.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://ffw.zhongyouzk.top

Go:   os.Getwd()
来源：http://njh.gogol.net.cn

Ruby: Dir.pwd
来源：http://tvo.tianlin.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://nmb.cqqwz.cn

[M05] 设置退出码
来源：http://irk.bbcook.cn

Py:   sys.exit(1)
来源：http://qes.mhx1999.top

PHP:  exit(1);
来源：http://guu.yangfankeji.com

JS:   process.exit(1)
来源：http://yzt.cdnleiting.top

TS:   process.exit(1)
来源：http://yky.zhaomingkeji.xyz

Java: System.exit(1)
来源：http://kog.tarul.cn

Go:   os.Exit(1)
来源：http://bxi.0kj1m.cn

Ruby: exit 1
来源：http://wln.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dxv.redwolf501.top

[M06] 向标准错误输出
来源：http://ket.jinqigufen.top

Py:   print("err", file=sys.stderr)
来源：http://wfv.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fzp.tianlin.xyz

JS:   console.error("err")
来源：http://tbh.uphjek.com

TS:   console.error("err")
来源：http://ney.xinyue.icu

Java: System.err.println("err")
来源：http://uta.smart0.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ihk.zhiwuduotai.top

Ruby: warn "err"
来源：http://stg.chenjidiqi.icu

C#:   Console.Error.WriteLine("err")
来源：http://qvl.c1oappe.top

[M07] 判断是否为主入口
来源：http://sky.dianchejie.cn

Py:   if __name__ == "__main__":
来源：http://ytp.svipenyu.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xoi.zhongyouzk.top

JS:   require.main === module
来源：http://rnw.andypj.xyz

TS:   require.main === module
来源：http://bkd.smart0.xyz

Java: public static void main(String[] args)
来源：http://sev.kuanghao11.cn

Go:   func main()
来源：http://vtb.cheryme.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://shb.pycfn.com

C#:   static void Main(string[] args)
来源：http://xxl.zhiwuduotai.top

[M08] 获取系统与运行时信息
来源：http://bzi.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://lwh.feifeiyinyue.top

PHP:  PHP_OS;  phpversion();
来源：http://acf.hfpthk.cn

JS:   process.platform;  process.version
来源：http://lbu.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://tto.nwbrower.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mxu.ydzc1.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xdc.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vnx.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://zqr.chenjidiqi.icu

================================================================================
来源：http://yvt.chenzaomai.com

N. 数据结构与算法
来源：http://uuz.ydjk.org.cn

================================================================================
来源：http://uff.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://lvz.c1oappe.top

Py:   bisect.bisect_left(arr, x)
来源：http://gay.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://qle.ivvv.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ysk.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://aab.shangyingyoupin.top

Java: Arrays.binarySearch(arr, x)
来源：http://uky.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://gmp.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://dlm.hongshengwenyu.top

C#:   Array.BinarySearch(arr, x)
来源：http://tsz.sweek.top

[N02] 排序（工程实践用内置实现）
来源：http://pge.dashuyun.cn

Py:   sorted(arr);  arr.sort()
来源：http://fdj.gotoacloud.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ont.cheryme.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://soo.xinyue.icu

TS:   [...arr].sort((a, b) => a - b)
来源：http://mdx.sysykeji.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fsl.c1oappe.top

Go:   slices.Sort(arr)
来源：http://pjf.yfazqb.com

Ruby: arr.sort
来源：http://sis.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://xvi.yj20258.top

[N03] 快速排序（分治示例）
来源：http://eie.shzxlz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jfc.nanxinkj.top

PHP:  // 递归实现，或用 usort
来源：http://hyl.hesvh.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wau.nanxuanxn.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://skh.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mnx.shangyingyoupin.top


<!-- 参考信息 -->