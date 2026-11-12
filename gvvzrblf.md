代发 wailian999

Py:   (end - start).total_seconds()
来源：http://xlk.xinyue.icu

PHP:  $end->diff($start)->days;
来源：http://lue.hysaishi.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://dvm.aibaodan.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://ulw.wangshuangyany.cn

Java: Duration.between(start, end).toSeconds()
来源：http://ayi.gogol.net.cn

Go:   end.Sub(start).Hours()
来源：http://hhe.shuidangran.top

Ruby: end - start                 # 返回秒数
来源：http://ums.cdnleiting.top

C#:   (end - start).TotalSeconds
来源：http://rsc.jinqigfzy.top

[J07] 比较两个日期
来源：http://uax.quarkkingdee.top

Py:   d1 < d2;  d1 == d2
来源：http://jvh.svipenyu.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sov.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://uut.havefunace.top

TS:   d1.getTime() < d2.getTime()
来源：http://iei.kuanghao11.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://uvm.jqgufenzy.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zxd.jianghu66.top

Ruby: d1 < d2;  d1 == d2
来源：http://wki.shangyingyoupin.top

C#:   d1 < d2;  d1 == d2
来源：http://qnm.daria6918.cn

[J08] 提取年月日与星期
来源：http://mrd.hesvh.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://czy.yangfankeji.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://rdf.nanxinkj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://xnz.yfazqb.com

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://spx.havefunace.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pgt.gaohongyu789.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://osn.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://nno.cdnleiting.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://uvd.shangyingyoupin.top

[J09] 时区处理
来源：http://hjm.xziqi.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://loz.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://heo.uphjek.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://edd.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qsa.yanxiufei.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rih.hesvh.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://tak.shanyushiyangkeji.top

Ruby: Time.now.getlocal("+08:00")
来源：http://yqt.andypj.xyz

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ooy.fzhhl.top

[J10] 取今天 / 本月第一天
来源：http://xwl.xziqi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tas.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://nvh.zhiwuduotai.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gyt.fzhhl.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vea.tian-w.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://egy.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tih.iojbl.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://msz.svipenyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://azk.mhx1999.top

================================================================================
来源：http://bwe.havefunace.top

K. JSON 与序列化
来源：http://uvz.hammf.cn

================================================================================
来源：http://gas.redwolf501.top

[K01] 对象转 JSON 字符串
来源：http://fat.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://sod.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zzu.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://vvs.cheryme.top

TS:   JSON.stringify(obj)
来源：http://dqg.gogol.net.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nwd.yfazqb.com

Go:   json.Marshal(obj)
来源：http://gth.yuanzhike.top

Ruby: obj.to_json                                     // require "json"
来源：http://tfo.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ctd.havefunace.top

[K02] JSON 字符串转对象
来源：http://flm.zhixingplan.top

Py:   json.loads(s)
来源：http://gjq.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://etr.guannengcc.top

JS:   JSON.parse(s)
来源：http://kpi.vehdjk.com

TS:   JSON.parse(s)
来源：http://xrc.cashguo.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ngi.chenlongwang.top

Go:   json.Unmarshal(data, &v)
来源：http://azk.zhiwuduotai.top

Ruby: JSON.parse(s)
来源：http://fgu.hysaishi.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rdp.cheryme.top

[K03] JSON 美化输出（带缩进）
来源：http://nce.birdmap.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uzm.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pma.jqgfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://ayv.jqgufenzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hwi.yj202588.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oqf.hesvh.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ond.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://osa.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://fdw.bjfxy.top

[K04] 读取 JSON 文件
来源：http://muv.feifeiyinyue.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xyl.hnqzz.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://myl.havefunace.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wrq.yj202588.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tcn.ctjpmb.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://keu.zhaomingkeji.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vxr.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://epf.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aux.fzhhl.top

[K05] 深拷贝对象
来源：http://med.zhiwuduotai.top

Py:   copy.deepcopy(obj)
来源：http://qjp.feifeiyinyue.top

PHP:  unserialize(serialize($obj));
来源：http://khi.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://mtb.ybcxt.top

TS:   structuredClone(obj)
来源：http://zgh.chenjidiqi.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://zpk.jiagoushi.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://txq.jiagoushi.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://sdt.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nrz.havefunace.top

[K06] 解析 URL 查询串
来源：http://ucy.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://drf.316326.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qmu.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://brn.yfazqb.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://oww.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ype.hammf.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dzi.316326.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://umw.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://koo.tanke756.top

[K07] 进制转换
来源：http://qab.jyoumei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gdv.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ckm.yj20258888.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vwo.jqgfzy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hgc.zhengqikj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bgd.shanyushiyangkeji.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://phh.mhx1999.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eru.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yjg.jianghu66.top

[K08] 二进制序列化（非 JSON）
来源：http://zic.tanke756.top

Py:   pickle.dumps(obj)
来源：http://xvs.zhaomingkeji.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://wwq.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://afy.zhiwuduotai.top

TS:   v8.serialize(obj)        // Node
来源：http://csa.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://sgs.nanxuanxn.top

Go:   encoding/gob
来源：http://nsi.zhengqikj.top

Ruby: Marshal.dump(obj)
来源：http://uab.ydjk.org.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zev.zhengqikj.top

================================================================================
来源：http://rhl.yuanzhike.top

L. 网络请求
来源：http://wrg.smart0.xyz

================================================================================
来源：http://wqg.tianlin.xyz

[L01] 发送 GET 请求
来源：http://epz.hywenlv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://smf.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ypd.zhongyouzk.top

JS:   await fetch(url)
来源：http://adc.daria6918.cn

TS:   await fetch(url)
来源：http://hos.zycfv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://epr.ydzc1.top

Go:   resp, err := http.Get(url)
来源：http://ejj.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://tmh.hysaishi.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xfl.hcnkem.com

[L02] 发送 POST JSON
来源：http://xjr.cqqwz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ehv.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://efx.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cun.jianghu66.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oyz.zdbjq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://glm.jqgufenzy.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nlx.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mok.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://vyx.pycfn.com

[L03] 设置自定义请求头
来源：http://yri.hywenlv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tbm.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vdy.meibo888.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wle.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ymf.sjlbkw.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wch.guannengcc.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wkl.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ldt.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://eiy.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://zjz.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://iir.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wjq.shanyushiyangtech.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qou.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nba.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yps.xuetiantiany.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ofl.smart0.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yhe.jqgufenzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xtm.yuxming.cn

[L05] 上传文件（multipart）
来源：http://jva.jinqigufen.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://sba.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bay.hcnkem.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xhe.jinyuanbaomall.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://otk.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jdp.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jgf.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://svb.xuetiantiany.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vjo.fehbvm.com

[L06] 解析响应为 JSON
来源：http://gwg.52xcode.cn

Py:   resp.json()
来源：http://bsn.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://cdw.snrcjt.cn

JS:   await resp.json()
来源：http://ofy.tanke756.top

TS:   await resp.json()
来源：http://ura.hnxiangtu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cte.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kjo.vqdsnc.cn

Ruby: JSON.parse(resp.body)
来源：http://sry.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nhc.hysaishi.cn

[L07] 处理 HTTP 状态码
来源：http://hws.52xcode.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rse.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://iid.yuanzhike.top

JS:   resp.ok;  resp.status
来源：http://kcl.quarkkingdee.top

TS:   resp.ok;  resp.status
来源：http://uga.ppjwa.cn

Java: resp.statusCode()
来源：http://mdu.cashguo.top

Go:   resp.StatusCode
来源：http://qhy.fzhhl.top

Ruby: resp.code.to_i
来源：http://unt.aizwys.cn

C#:   (int)resp.StatusCode
来源：http://nmz.yuanzhike.top

[L08] 并发请求多个地址
来源：http://euu.fzhhl.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://btx.pycfn.com

PHP:  curl_multi_init() 系列
来源：http://phz.yuxming.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://crv.chenlongwang.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jdd.jiagoushi.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://sde.nwbrower.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iyb.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://six.zhoulong.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vxh.uphjek.com

================================================================================
来源：http://iiw.pengpengdd.cyou

M. 命令行 / 进程 / 环境
来源：http://ctp.chenjidiqi.icu

================================================================================
来源：http://vbu.meibo888.top

[M01] 读取命令行参数
来源：http://jeb.guowangkeji.top

Py:   sys.argv[1:]
来源：http://pir.yfazqb.com

PHP:  $argv;  $argc;
来源：http://may.xingfuxueyuan.xyz

JS:   process.argv.slice(2)
来源：http://oli.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://ttu.nwbrower.top

Java: args 数组（main 方法参数）
来源：http://oju.gotoacloud.top

Go:   os.Args[1:]
来源：http://gro.zhijiandao.cn

Ruby: ARGV
来源：http://oeu.birdmap.top

C#:   args 数组（Main 方法参数）
来源：http://khg.xylfe.cn

[M02] 读取环境变量
来源：http://fbi.yangfankeji.com

Py:   os.environ.get("HOME")
来源：http://wpb.c1oappe.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lov.hammf.cn

JS:   process.env.HOME
来源：http://bkt.zhengqikj.top

TS:   process.env.HOME
来源：http://wcx.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://ggi.jianghu66.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ysj.bjfxy.top

Ruby: ENV["HOME"]
来源：http://wsz.yangfankeji.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nbi.fengsongda.top

[M03] 执行外部命令
来源：http://mfq.redwolf501.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wdy.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jju.nanxuanxn.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xkl.chenjidiqi.icu

TS:   child_process.execSync("ls -l").toString()
来源：http://iju.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fye.gaohongyu789.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ceh.guowangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://dbl.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://jvd.xziqi.cn

[M04] 获取当前工作目录
来源：http://kvs.hnxiangtu.top

Py:   os.getcwd()
来源：http://hkp.yuxming.cn

PHP:  getcwd();
来源：http://wat.hnqzz.top

JS:   process.cwd()
来源：http://ecq.kuanghao11.cn

TS:   process.cwd()
来源：http://bto.vehdjk.com

Java: Path.of("").toAbsolutePath()
来源：http://biz.xuetiantiany.cn

Go:   os.Getwd()
来源：http://cbb.fktsv.cn

Ruby: Dir.pwd
来源：http://nyk.chenzaomai.com

C#:   Directory.GetCurrentDirectory()
来源：http://cgd.daria6918.cn

[M05] 设置退出码
来源：http://tlp.yanxiufei.cn

Py:   sys.exit(1)
来源：http://ecx.yuanzhike.top

PHP:  exit(1);
来源：http://qhr.guannengcc.top

JS:   process.exit(1)
来源：http://wqs.jinyuanbaomall.cn

TS:   process.exit(1)
来源：http://ycx.jinqigfzy.top

Java: System.exit(1)
来源：http://frt.gogol.net.cn

Go:   os.Exit(1)
来源：http://myv.yj202588.top

Ruby: exit 1
来源：http://wrf.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kqi.hnqzz.top

[M06] 向标准错误输出
来源：http://gns.316326.xyz

Py:   print("err", file=sys.stderr)
来源：http://jkx.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://jub.jinqigufen.top

JS:   console.error("err")
来源：http://dog.yueranfly.top

TS:   console.error("err")
来源：http://www.meibo888.top

Java: System.err.println("err")
来源：http://rar.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://vda.feifeiyinyue.top

Ruby: warn "err"
来源：http://eda.gaohongyu789.top

C#:   Console.Error.WriteLine("err")
来源：http://ifw.snrcjt.cn

[M07] 判断是否为主入口
来源：http://nkp.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://lei.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ydi.epnwcf.com

JS:   require.main === module
来源：http://lai.yangfankeji.com

TS:   require.main === module
来源：http://vho.zhixingplan.top

Java: public static void main(String[] args)
来源：http://bfi.zhixingplan.top

Go:   func main()
来源：http://eqd.ivvv.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nwh.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://pmp.zhengqikj.top

[M08] 获取系统与运行时信息
来源：http://sjf.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://qub.fzhhl.top

PHP:  PHP_OS;  phpversion();
来源：http://rmg.cdnleiting.top

JS:   process.platform;  process.version
来源：http://cmy.sufxvd.cn

TS:   process.platform;  process.version
来源：http://zvx.iojbl.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gkk.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zar.svipenyu.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jzt.zycfv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ech.jqgfzy.top

================================================================================
来源：http://ein.cashguo.top

N. 数据结构与算法
来源：http://oli.jiagoushi.top

================================================================================
来源：http://bpa.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://ita.dianchejie.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ppi.jinqigfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ihx.jianghu66.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bin.sweek.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://bzm.zhijiandao.cn

Java: Arrays.binarySearch(arr, x)
来源：http://vxu.zycfv.cn

Go:   sort.SearchInts(arr, x)
来源：http://dab.pycfn.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://hyk.aizwys.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bbg.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://oqt.xuanzx.com

Py:   sorted(arr);  arr.sort()
来源：http://zkq.zhengqikj.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xbe.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://qsp.yj202588.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ypl.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://emm.cdnleiting.top

Go:   slices.Sort(arr)
来源：http://dae.aizwys.cn

Ruby: arr.sort
来源：http://xej.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://dzr.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://eeo.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://msc.hesvh.cn

PHP:  // 递归实现，或用 usort
来源：http://dmk.daria6918.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ggu.andypj.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gnb.sweek.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zck.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wvr.yj20258888.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rae.hfpthk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://yte.fktsv.cn

[N04] 斐波那契数列
来源：http://kyb.zhongyouzk.top


<!-- 参考信息 -->