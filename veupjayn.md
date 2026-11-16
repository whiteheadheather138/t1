代发 wailian999

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://upx.sysykeji.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://ijg.dashuyun.cn

[J05] 时间加减（加 7 天）
来源：http://adc.aizwys.cn

Py:   now + timedelta(days=7)
来源：http://zfw.haohaochexian.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://pej.316326.xyz

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://fzm.hammf.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://bqm.cashguo.top

Java: LocalDate.now().plusDays(7)
来源：http://maj.tian-w.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://tbl.andypj.xyz

Ruby: Time.now + 7 * 86400
来源：http://czz.9152youxi.cn

C#:   DateTime.Now.AddDays(7)
来源：http://qqp.xylfe.cn

[J06] 计算两时间之差
来源：http://dif.yangfankeji.com

Py:   (end - start).total_seconds()
来源：http://zma.xylfe.cn

PHP:  $end->diff($start)->days;
来源：http://gwd.xingfuxueyuan.xyz

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pll.c1oappe.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://kep.xylfe.cn

Java: Duration.between(start, end).toSeconds()
来源：http://fpv.316326.xyz

Go:   end.Sub(start).Hours()
来源：http://bnp.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://jyo.vehdjk.com

C#:   (end - start).TotalSeconds
来源：http://rkm.uphjek.com

[J07] 比较两个日期
来源：http://xmc.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://vtn.sxryk.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wyp.9152youxi.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lug.0kj1m.cn

TS:   d1.getTime() < d2.getTime()
来源：http://wdp.gzhubu.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fwf.xingfuxueyuan.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pce.hesvh.cn

Ruby: d1 < d2;  d1 == d2
来源：http://ioq.dashuyun.cn

C#:   d1 < d2;  d1 == d2
来源：http://pkz.shanyushiyangkeji.top

[J08] 提取年月日与星期
来源：http://kya.yueranfly.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gar.fktsv.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ulq.0kj1m.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://eth.snrcjt.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://aov.9152youxi.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://atx.yuanzhike.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://aux.tarul.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://bvr.xziqi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://oos.hammf.cn

[J09] 时区处理
来源：http://mcl.svipenyu.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://blx.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://sxs.epnwcf.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jvr.yj20258.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xbo.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://plj.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kxw.ywan-chungtsiang.top

Ruby: Time.now.getlocal("+08:00")
来源：http://jat.nanxuanxn.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gfn.hcnkem.com

[J10] 取今天 / 本月第一天
来源：http://zsp.sysykeji.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tfw.yuxming.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vhy.sweek.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://lop.c1oappe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ikz.shzxlz.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://avh.9152youxi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gki.zdbjq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xtv.yj202588.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://quv.c1oappe.top

================================================================================
来源：http://lom.shanyushiyangkeji.top

K. JSON 与序列化
来源：http://jnv.vqdsnc.cn

================================================================================
来源：http://uuz.sufxvd.cn

[K01] 对象转 JSON 字符串
来源：http://rgm.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vpv.sufxvd.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ldj.cashguo.top

JS:   JSON.stringify(obj)
来源：http://oux.yanxiufei.cn

TS:   JSON.stringify(obj)
来源：http://pnk.ybcxt.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ewa.hnqzz.top

Go:   json.Marshal(obj)
来源：http://bxs.hywenlv.cn

Ruby: obj.to_json                                     // require "json"
来源：http://sfl.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://gao.cdnleiting.top

[K02] JSON 字符串转对象
来源：http://dgz.zhengqikj.top

Py:   json.loads(s)
来源：http://tlo.guowangkeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fab.snrcjt.cn

JS:   JSON.parse(s)
来源：http://woc.xziqi.cn

TS:   JSON.parse(s)
来源：http://zix.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hip.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://iht.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://zgp.xuanzx.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bvi.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://vjn.yueranfly.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://vus.aibaodan.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dui.sweek.top

JS:   JSON.stringify(obj, null, 2)
来源：http://sao.xylfe.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://puk.ybcxt.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eds.tian-w.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rlj.tianlin.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://pax.gogol.net.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pim.xinyue.icu

[K04] 读取 JSON 文件
来源：http://oxz.cdnleiting.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ial.xuetiantiany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ixm.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tws.yonumen.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zkx.hywenlv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mtz.snrcjt.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://snr.ehwqpu.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ejd.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lon.hammf.cn

[K05] 深拷贝对象
来源：http://szv.fzhhl.top

Py:   copy.deepcopy(obj)
来源：http://kfc.fehbvm.com

PHP:  unserialize(serialize($obj));
来源：http://ecv.hywenlv.cn

JS:   structuredClone(obj)
来源：http://lyk.nanxinkj.top

TS:   structuredClone(obj)
来源：http://juz.haohaochexian.top

Java: // 手写拷贝构造，或序列化往返
来源：http://fip.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jrs.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://omn.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://cie.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://wal.shanyushiyangtech.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rbf.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://bnb.jinqigufen.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://emv.9152youxi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lxh.shzxlz.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://pam.hnxiangtu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://bnt.fktsv.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://wzn.xuetiantiany.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://esk.cucudq.cn

[K07] 进制转换
来源：http://tik.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dyk.yj20258.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hzl.zhixingplan.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://cpw.c1oappe.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ldb.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vos.pycfn.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://gjg.hesvh.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nbj.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wuw.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://jdg.zdqjudy.top

Py:   pickle.dumps(obj)
来源：http://xfw.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://fff.tarul.cn

JS:   v8.serialize(obj)        // Node
来源：http://knu.yj20258888.top

TS:   v8.serialize(obj)        // Node
来源：http://gsw.guowangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://wks.tianlin.xyz

Go:   encoding/gob
来源：http://ich.dashuyun.cn

Ruby: Marshal.dump(obj)
来源：http://tmi.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jxz.sysykeji.top

================================================================================
来源：http://vkl.kuanghao11.cn

L. 网络请求
来源：http://zhu.ppjwa.cn

================================================================================
来源：http://lpp.uphjek.com

[L01] 发送 GET 请求
来源：http://fdq.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mgo.ppjwa.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pec.aibaodan.cn

JS:   await fetch(url)
来源：http://jgb.zhongyouzk.top

TS:   await fetch(url)
来源：http://itm.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bdz.zdbjq.cn

Go:   resp, err := http.Get(url)
来源：http://xuy.epnwcf.com

Ruby: Net::HTTP.get(URI(url))
来源：http://uyi.9152youxi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bft.zdbjq.cn

[L02] 发送 POST JSON
来源：http://mxx.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://tix.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zqm.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zsv.ybcxt.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ftp.havefunace.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dtm.birdmap.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://oet.shzxlz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://quz.tianlin.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wef.daxiang520.top

[L03] 设置自定义请求头
来源：http://wot.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://sdu.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://umo.nanxuanxn.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jxy.hammf.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://itl.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vun.zhongyouzk.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://flp.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://uvq.tian-w.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yos.9152youxi.cn

[L04] 设置超时
来源：http://ljw.jqgufenzy.top

Py:   requests.get(url, timeout=5)
来源：http://ylu.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ejb.zhijiandao.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wix.ydzc1.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yie.gzhubu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://evl.ydzc1.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ghz.fehbvm.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tki.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yzu.redwolf501.top

[L05] 上传文件（multipart）
来源：http://lei.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eoo.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://xqp.shanyushiyangtech.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://gcv.c1oappe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://yfy.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nkd.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://itu.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lko.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://nnc.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://cgh.nwbrower.top

Py:   resp.json()
来源：http://qtx.yonumen.top

PHP:  json_decode($body, true);
来源：http://xtf.tian-w.cn

JS:   await resp.json()
来源：http://amy.fanxiaobao.xyz

TS:   await resp.json()
来源：http://dmw.jyoumei.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cas.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wvh.zhaomingkeji.xyz

Ruby: JSON.parse(resp.body)
来源：http://hhp.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://duz.meibo888.top

[L07] 处理 HTTP 状态码
来源：http://iod.yanxiufei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ifu.yuanzhike.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://klq.daxiang520.top

JS:   resp.ok;  resp.status
来源：http://nxm.iojbl.cn

TS:   resp.ok;  resp.status
来源：http://lsn.jyoumei.cn

Java: resp.statusCode()
来源：http://fsd.cheryme.top

Go:   resp.StatusCode
来源：http://oze.cdnleiting.top

Ruby: resp.code.to_i
来源：http://cpx.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://vrl.uphjek.com

[L08] 并发请求多个地址
来源：http://cba.jlsjyb.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://pfp.svipenyu.cn

PHP:  curl_multi_init() 系列
来源：http://rhq.c1oappe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mpw.shzxlz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jcl.xuanzx.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://zri.xinyue.icu

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://dlo.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qtz.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rsi.hongshengwenyu.top

================================================================================
来源：http://nir.tianlin.xyz

M. 命令行 / 进程 / 环境
来源：http://ovn.andypj.xyz

================================================================================
来源：http://tuk.yj20258.top

[M01] 读取命令行参数
来源：http://uhv.haohaochexian.top

Py:   sys.argv[1:]
来源：http://xvm.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://wod.jyoumei.cn

JS:   process.argv.slice(2)
来源：http://xjc.zhijiandao.cn

TS:   process.argv.slice(2)
来源：http://erf.mhx1999.top

Java: args 数组（main 方法参数）
来源：http://rcr.xinyue.icu

Go:   os.Args[1:]
来源：http://wkh.xylfe.cn

Ruby: ARGV
来源：http://cye.shanyushiyangtech.top

C#:   args 数组（Main 方法参数）
来源：http://kdk.vehdjk.com

[M02] 读取环境变量
来源：http://xdf.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://fua.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tht.aizwys.cn

JS:   process.env.HOME
来源：http://vcr.gogol.net.cn

TS:   process.env.HOME
来源：http://tld.yvedp.cn

Java: System.getenv("HOME")
来源：http://nxf.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pbc.ehwqpu.com

Ruby: ENV["HOME"]
来源：http://afc.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://flc.guowangkeji.top

[M03] 执行外部命令
来源：http://myt.guowangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ntb.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qvp.ehwqpu.com

JS:   child_process.execSync("ls -l").toString()
来源：http://axt.pengpengdd.cyou

TS:   child_process.execSync("ls -l").toString()
来源：http://gyy.316326.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://iyf.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jna.shzxlz.cn

Ruby: system("ls -l");  `ls -l`
来源：http://zav.sxryk.cn

C#:   Process.Start("ls", "-l");
来源：http://htx.hywenlv.cn

[M04] 获取当前工作目录
来源：http://mle.pycfn.com

Py:   os.getcwd()
来源：http://opm.zhaomingkeji.xyz

PHP:  getcwd();
来源：http://lqy.yuanzhike.top

JS:   process.cwd()
来源：http://idv.yangfankeji.com

TS:   process.cwd()
来源：http://aak.ppjwa.cn

Java: Path.of("").toAbsolutePath()
来源：http://wim.cheryme.top

Go:   os.Getwd()
来源：http://avo.jinyuanbaomall.cn

Ruby: Dir.pwd
来源：http://phs.svipenyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://rhs.ctjpmb.com

[M05] 设置退出码
来源：http://xnw.fktsv.cn

Py:   sys.exit(1)
来源：http://ris.smart0.xyz

PHP:  exit(1);
来源：http://msl.xinyue.icu

JS:   process.exit(1)
来源：http://tqf.xziqi.cn

TS:   process.exit(1)
来源：http://wxf.tian-w.cn

Java: System.exit(1)
来源：http://ssc.chenjidiqi.icu

Go:   os.Exit(1)
来源：http://tba.jinyuanbaomall.cn

Ruby: exit 1
来源：http://xtq.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://edi.yfazqb.com

[M06] 向标准错误输出
来源：http://rje.cashguo.top

Py:   print("err", file=sys.stderr)
来源：http://dfc.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kpp.sjlbkw.cn

JS:   console.error("err")
来源：http://czz.yuxming.cn

TS:   console.error("err")
来源：http://won.yangfankeji.com

Java: System.err.println("err")
来源：http://brv.jinqigfzy.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://xii.hywenlv.cn

Ruby: warn "err"
来源：http://nma.sufxvd.cn

C#:   Console.Error.WriteLine("err")
来源：http://qjj.yj202588.top

[M07] 判断是否为主入口
来源：http://hli.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://jdf.zycfv.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bhv.feifeiyinyue.top

JS:   require.main === module
来源：http://peo.ehwqpu.com

TS:   require.main === module
来源：http://vvf.zycfv.cn

Java: public static void main(String[] args)
来源：http://wsy.wangdashe.top

Go:   func main()
来源：http://klx.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vkc.jiagoushi.top

C#:   static void Main(string[] args)
来源：http://sdl.nwbrower.top

[M08] 获取系统与运行时信息
来源：http://tas.zhiwuduotai.top

Py:   platform.system();  platform.python_version()
来源：http://dyd.c1oappe.top

PHP:  PHP_OS;  phpversion();
来源：http://ecd.daria6918.cn

JS:   process.platform;  process.version
来源：http://jev.pengpengdd.cyou

TS:   process.platform;  process.version
来源：http://buv.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://dhw.hnqzz.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://gmv.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xoo.bbcook.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://kyv.aibaodan.cn

================================================================================
来源：http://cim.52xcode.cn

N. 数据结构与算法
来源：http://wgi.zhoulong.xyz

================================================================================
来源：http://puj.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://hiy.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://tsq.yongpay.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wuf.zhiwuduotai.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nre.zhijiandao.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qsi.aizwys.cn

Java: Arrays.binarySearch(arr, x)
来源：http://azj.jianghu66.top

Go:   sort.SearchInts(arr, x)
来源：http://yco.aibaodan.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ffg.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://egb.aibaodan.cn

[N02] 排序（工程实践用内置实现）
来源：http://zdz.ywan-chungtsiang.top

Py:   sorted(arr);  arr.sort()
来源：http://xpn.hnxiangtu.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://svd.zhiwuduotai.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://aie.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://yte.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://plq.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://rfr.yanxiufei.cn


<!-- 参考信息 -->