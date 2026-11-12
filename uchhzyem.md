代发 wailian999

PHP:  (new DateTime())->modify("+7 days");
来源：http://uib.dashuyun.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://eqc.c1oappe.top

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://dvj.yvedp.cn

Java: LocalDate.now().plusDays(7)
来源：http://zuj.sweek.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://gky.ybcxt.top

Ruby: Time.now + 7 * 86400
来源：http://bxd.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://ylu.zhaomingkeji.xyz

[J06] 计算两时间之差
来源：http://gpo.dianchejie.cn

Py:   (end - start).total_seconds()
来源：http://ahr.smart0.xyz

PHP:  $end->diff($start)->days;
来源：http://wkm.iojbl.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://ysm.bbcook.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://nkq.yanxiufei.cn

Java: Duration.between(start, end).toSeconds()
来源：http://jgs.yonumen.top

Go:   end.Sub(start).Hours()
来源：http://njk.xylfe.cn

Ruby: end - start                 # 返回秒数
来源：http://qjs.sufxvd.cn

C#:   (end - start).TotalSeconds
来源：http://ldj.tarul.cn

[J07] 比较两个日期
来源：http://bgt.pycfn.com

Py:   d1 < d2;  d1 == d2
来源：http://xug.zhiwuduotai.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://hfv.fengsongda.top

JS:   d1.getTime() < d2.getTime()
来源：http://mkg.shanyushiyangtech.top

TS:   d1.getTime() < d2.getTime()
来源：http://acd.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ssf.fzhhl.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://euu.gogol.net.cn

Ruby: d1 < d2;  d1 == d2
来源：http://czk.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://vsh.yangfankeji.com

[J08] 提取年月日与星期
来源：http://oxd.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bsn.guannengcc.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://tad.yanxiufei.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://aiq.hesvh.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xdz.shanyushiyangtech.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tqo.fzhhl.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ypi.sxryk.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://iuc.ydzc1.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://jes.shanyushiyangkeji.top

[J09] 时区处理
来源：http://pmc.fktsv.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://byn.9152youxi.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://grf.snrcjt.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uaw.birdmap.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gub.cashguo.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://egz.tian-w.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nja.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cct.zhongyouzk.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eqz.uphjek.com

[J10] 取今天 / 本月第一天
来源：http://xvm.fehbvm.com

Py:   date.today();  date.today().replace(day=1)
来源：http://nmb.redwolf501.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://mpi.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kus.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ibg.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://trf.hammf.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://taa.zhijiandao.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mcv.9152youxi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bub.yangfankeji.com

================================================================================
来源：http://pgq.fzhhl.top

K. JSON 与序列化
来源：http://ttc.yanxiufei.cn

================================================================================
来源：http://frq.daxiang520.top

[K01] 对象转 JSON 字符串
来源：http://sac.bjfxy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wne.pycfn.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xxq.snrcjt.cn

JS:   JSON.stringify(obj)
来源：http://owv.316326.xyz

TS:   JSON.stringify(obj)
来源：http://qsa.fzhhl.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://uwi.cucudq.cn

Go:   json.Marshal(obj)
来源：http://jol.pycfn.com

Ruby: obj.to_json                                     // require "json"
来源：http://lgg.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kkd.hesvh.cn

[K02] JSON 字符串转对象
来源：http://tpr.ehwqpu.com

Py:   json.loads(s)
来源：http://cxw.gotoacloud.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dra.yuanzhike.top

JS:   JSON.parse(s)
来源：http://itt.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://jry.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ivm.9152youxi.cn

Go:   json.Unmarshal(data, &v)
来源：http://twu.zhijiandao.cn

Ruby: JSON.parse(s)
来源：http://msk.pycfn.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://nyp.jqgufenzy.top

[K03] JSON 美化输出（带缩进）
来源：http://dan.yj20258.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hvv.cqqwz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://upv.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://bzn.ppjwa.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fpw.haohaochexian.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xux.xuanzx.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kbe.gogol.net.cn

Ruby: JSON.pretty_generate(obj)
来源：http://mqe.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lgu.jianghu66.top

[K04] 读取 JSON 文件
来源：http://fwv.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pgv.hnxiangtu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://enx.hesvh.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jji.zhiwuduotai.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cbr.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vrq.havefunace.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://unl.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://dhs.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vde.jianghu66.top

[K05] 深拷贝对象
来源：http://gwz.zhaomingkeji.xyz

Py:   copy.deepcopy(obj)
来源：http://cts.yj20258.top

PHP:  unserialize(serialize($obj));
来源：http://xse.jinqigufen.top

JS:   structuredClone(obj)
来源：http://lqb.pycfn.com

TS:   structuredClone(obj)
来源：http://ump.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vbi.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nla.svipenyu.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xzt.bbcook.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://acd.vqdsnc.cn

[K06] 解析 URL 查询串
来源：http://gls.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://bog.fehbvm.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://efl.mhx1999.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bon.yangfankeji.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ryq.guowangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gxj.haohaochexian.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://uhe.zhijiandao.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fwt.52xcode.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gzz.gotoacloud.top

[K07] 进制转换
来源：http://ekx.hongshengwenyu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ugj.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://woa.gotoacloud.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pnb.chenjidiqi.icu

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pim.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dpu.zhengqikj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://itc.smart0.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mhh.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bym.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://xhu.jqgfzy.top

Py:   pickle.dumps(obj)
来源：http://nth.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://pjo.hywenlv.cn

JS:   v8.serialize(obj)        // Node
来源：http://bkw.hfpthk.cn

TS:   v8.serialize(obj)        // Node
来源：http://skc.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ays.xingfuxueyuan.xyz

Go:   encoding/gob
来源：http://htr.fehbvm.com

Ruby: Marshal.dump(obj)
来源：http://xsx.yongpay.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ble.hnqzz.top

================================================================================
来源：http://wdl.yueranfly.top

L. 网络请求
来源：http://nvv.redwolf501.top

================================================================================
来源：http://lvx.fktsv.cn

[L01] 发送 GET 请求
来源：http://ixn.jianghu66.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://arw.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jwo.yanxiufei.cn

JS:   await fetch(url)
来源：http://ybv.zycfv.cn

TS:   await fetch(url)
来源：http://hqw.guannengcc.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oer.chenjidiqi.icu

Go:   resp, err := http.Get(url)
来源：http://zdv.daxiang520.top

Ruby: Net::HTTP.get(URI(url))
来源：http://dbk.mhx1999.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qsc.tian-w.cn

[L02] 发送 POST JSON
来源：http://obl.jianghu66.top

Py:   requests.post(url, json={"a": 1})
来源：http://smb.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uhm.ppjwa.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ece.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://prg.cdnleiting.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://huo.ppjwa.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ulr.guannengcc.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nof.gogol.net.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uyj.jianghu66.top

[L03] 设置自定义请求头
来源：http://vlk.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://omm.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jgf.ydzc1.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qzk.zhiwuduotai.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://eir.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uma.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://tfr.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zmy.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://xar.c1oappe.top

[L04] 设置超时
来源：http://cmc.chenzaomai.com

Py:   requests.get(url, timeout=5)
来源：http://iod.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://yfm.tian-w.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://szr.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gld.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nnz.hnqzz.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mki.jyoumei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://iug.zhiwuduotai.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://zyl.tianlin.xyz

[L05] 上传文件（multipart）
来源：http://qzw.epnwcf.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tsx.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bcw.c1oappe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://zxo.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://goc.fengsongda.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yjm.kuanghao11.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hvu.iojbl.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ddh.ybcxt.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rub.sufxvd.cn

[L06] 解析响应为 JSON
来源：http://xbv.ehwqpu.com

Py:   resp.json()
来源：http://uxc.hesvh.cn

PHP:  json_decode($body, true);
来源：http://yfx.zhongyouzk.top

JS:   await resp.json()
来源：http://frb.shzxlz.cn

TS:   await resp.json()
来源：http://jip.meibo888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vdw.guowangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ugh.sxryk.cn

Ruby: JSON.parse(resp.body)
来源：http://jxu.xingfuxueyuan.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gyl.zhixingplan.top

[L07] 处理 HTTP 状态码
来源：http://znf.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://guf.yj20258888.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zyc.sweek.top

JS:   resp.ok;  resp.status
来源：http://yoi.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://shf.hysaishi.cn

Java: resp.statusCode()
来源：http://qqo.yvedp.cn

Go:   resp.StatusCode
来源：http://cxm.hywenlv.cn

Ruby: resp.code.to_i
来源：http://ecf.mhx1999.top

C#:   (int)resp.StatusCode
来源：http://mfu.quarkkingdee.top

[L08] 并发请求多个地址
来源：http://xki.cdnleiting.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vxo.yongpay.top

PHP:  curl_multi_init() 系列
来源：http://qlv.nanxinkj.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tik.daria6918.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://aoj.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ath.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ovj.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://suy.gotoacloud.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hea.redwolf501.top

================================================================================
来源：http://xoi.fengsongda.top

M. 命令行 / 进程 / 环境
来源：http://vkj.vehdjk.com

================================================================================
来源：http://cgo.tian-w.cn

[M01] 读取命令行参数
来源：http://tvh.jiagoushi.top

Py:   sys.argv[1:]
来源：http://pbj.havefunace.top

PHP:  $argv;  $argc;
来源：http://gom.yvedp.cn

JS:   process.argv.slice(2)
来源：http://cxw.redwolf501.top

TS:   process.argv.slice(2)
来源：http://pti.fktsv.cn

Java: args 数组（main 方法参数）
来源：http://vrh.shanyushiyangkeji.top

Go:   os.Args[1:]
来源：http://oxm.aizwys.cn

Ruby: ARGV
来源：http://aax.cqqwz.cn

C#:   args 数组（Main 方法参数）
来源：http://rbk.quarkkingdee.top

[M02] 读取环境变量
来源：http://ztf.zhoulong.xyz

Py:   os.environ.get("HOME")
来源：http://tlk.shanyushiyangkeji.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://knl.ydjk.org.cn

JS:   process.env.HOME
来源：http://nuh.sxryk.cn

TS:   process.env.HOME
来源：http://gqv.sweek.top

Java: System.getenv("HOME")
来源：http://oae.pengpengdd.cyou

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tko.jinyuanbaomall.cn

Ruby: ENV["HOME"]
来源：http://buy.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://qai.tianlin.xyz

[M03] 执行外部命令
来源：http://teq.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://sah.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ocs.andypj.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://nqi.zhengqikj.top

TS:   child_process.execSync("ls -l").toString()
来源：http://diz.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xgz.cucudq.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://sac.ehwqpu.com

Ruby: system("ls -l");  `ls -l`
来源：http://yke.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://pqb.dianchejie.cn

[M04] 获取当前工作目录
来源：http://jii.yueranfly.top

Py:   os.getcwd()
来源：http://smi.andypj.xyz

PHP:  getcwd();
来源：http://ejg.hnxiangtu.top

JS:   process.cwd()
来源：http://myj.jinghuilouyu.cn

TS:   process.cwd()
来源：http://csk.zhixingplan.top

Java: Path.of("").toAbsolutePath()
来源：http://ops.shzxlz.cn

Go:   os.Getwd()
来源：http://nbw.hywenlv.cn

Ruby: Dir.pwd
来源：http://qau.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://plj.vqdsnc.cn

[M05] 设置退出码
来源：http://ftx.tarul.cn

Py:   sys.exit(1)
来源：http://oug.quarkkingdee.top

PHP:  exit(1);
来源：http://tqv.tianlin.xyz

JS:   process.exit(1)
来源：http://kjh.chenjidiqi.icu

TS:   process.exit(1)
来源：http://xdt.tian-w.cn

Java: System.exit(1)
来源：http://qxs.ydzc1.top

Go:   os.Exit(1)
来源：http://rbv.zhongyouzk.top

Ruby: exit 1
来源：http://lpk.birdmap.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hjr.cashguo.top

[M06] 向标准错误输出
来源：http://yrp.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://zwb.tanke756.top

PHP:  fwrite(STDERR, "err\n");
来源：http://uej.xziqi.cn

JS:   console.error("err")
来源：http://waw.yj20258.top

TS:   console.error("err")
来源：http://gbe.hcnkem.com

Java: System.err.println("err")
来源：http://kjh.yueranfly.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vua.hongshengwenyu.top

Ruby: warn "err"
来源：http://drj.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://kel.cqqwz.cn

[M07] 判断是否为主入口
来源：http://phu.feifeiyinyue.top

Py:   if __name__ == "__main__":
来源：http://fix.feifeiyinyue.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://afe.vqdsnc.cn

JS:   require.main === module
来源：http://amb.sysykeji.top

TS:   require.main === module
来源：http://fpc.redwolf501.top

Java: public static void main(String[] args)
来源：http://gff.zdbjq.cn

Go:   func main()
来源：http://edg.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://fdg.fehbvm.com

C#:   static void Main(string[] args)
来源：http://wja.yuanzhike.top

[M08] 获取系统与运行时信息
来源：http://lsr.cucudq.cn

Py:   platform.system();  platform.python_version()
来源：http://gyl.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://bmm.hnqzz.top

JS:   process.platform;  process.version
来源：http://xmx.shzxlz.cn

TS:   process.platform;  process.version
来源：http://teq.havefunace.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://jqd.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qzt.wangshuangyany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://hjt.shangyingyoupin.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fxn.pycfn.com

================================================================================
来源：http://lja.xingfuxueyuan.xyz

N. 数据结构与算法
来源：http://cpg.havefunace.top

================================================================================
来源：http://nev.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://hmw.shuidangran.top

Py:   bisect.bisect_left(arr, x)
来源：http://bpn.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iac.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hgz.yj20258.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://njn.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://ezr.cucudq.cn

Go:   sort.SearchInts(arr, x)
来源：http://kiq.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://sxt.cqqwz.cn

C#:   Array.BinarySearch(arr, x)
来源：http://jsm.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://frc.guowangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://pmx.gaohongyu789.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://pfi.bbcook.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://sau.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fkd.dashuyun.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fri.shangyingyoupin.top

Go:   slices.Sort(arr)
来源：http://xfv.yonumen.top

Ruby: arr.sort
来源：http://nbx.jiagoushi.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jxg.jqgufenzy.top

[N03] 快速排序（分治示例）
来源：http://ili.vqdsnc.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://bap.shanyushiyangtech.top


<!-- 参考信息 -->