代发 wailian999

Py:   (end - start).total_seconds()
来源：http://epc.hesvh.cn

PHP:  $end->diff($start)->days;
来源：http://nvm.ehwqpu.com

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://nuy.yangfankeji.com

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://yjg.hammf.cn

Java: Duration.between(start, end).toSeconds()
来源：http://lds.yuanzhike.top

Go:   end.Sub(start).Hours()
来源：http://siu.sxryk.cn

Ruby: end - start                 # 返回秒数
来源：http://oux.bjfxy.top

C#:   (end - start).TotalSeconds
来源：http://qin.birdmap.top

[J07] 比较两个日期
来源：http://vqg.uphjek.com

Py:   d1 < d2;  d1 == d2
来源：http://tye.yuxming.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://rad.ydjk.org.cn

JS:   d1.getTime() < d2.getTime()
来源：http://tpb.hcnkem.com

TS:   d1.getTime() < d2.getTime()
来源：http://wvg.tanke756.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://skz.gaohongyu789.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zgg.smart0.xyz

Ruby: d1 < d2;  d1 == d2
来源：http://iat.redwolf501.top

C#:   d1 < d2;  d1 == d2
来源：http://qox.yuxming.cn

[J08] 提取年月日与星期
来源：http://crm.guowangkeji.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xjt.yuxming.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://hyw.sxryk.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://kru.sysykeji.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://vbc.0kj1m.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yvm.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qzs.sysykeji.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://buw.nanxinkj.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://kdh.hnqzz.top

[J09] 时区处理
来源：http://tcg.hfpthk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dgi.jinghuilouyu.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rnf.zdqjudy.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://rls.iojbl.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://aug.sjlbkw.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://fcz.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://xvn.sweek.top

Ruby: Time.now.getlocal("+08:00")
来源：http://xav.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jiu.cqqwz.cn

[J10] 取今天 / 本月第一天
来源：http://gny.9152youxi.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://jae.sufxvd.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://tpg.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://eao.jqgufenzy.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://jtu.shuidangran.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://iiz.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://pdh.quarkkingdee.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://jxd.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nzb.tanke756.top

================================================================================
来源：http://nxc.kuanghao11.cn

K. JSON 与序列化
来源：http://mly.hesvh.cn

================================================================================
来源：http://cxa.svipenyu.cn

[K01] 对象转 JSON 字符串
来源：http://nmc.hysaishi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jzg.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jlk.zhijiandao.cn

JS:   JSON.stringify(obj)
来源：http://ubj.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://hga.smart0.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ecw.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://edt.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ioj.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hoh.yvedp.cn

[K02] JSON 字符串转对象
来源：http://fqo.yangfankeji.com

Py:   json.loads(s)
来源：http://gsr.uphjek.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://viu.dianchejie.cn

JS:   JSON.parse(s)
来源：http://qur.snrcjt.cn

TS:   JSON.parse(s)
来源：http://wqk.shangyingyoupin.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hzu.xuetiantiany.cn

Go:   json.Unmarshal(data, &v)
来源：http://dvx.fengsongda.top

Ruby: JSON.parse(s)
来源：http://klq.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://irq.andypj.xyz

[K03] JSON 美化输出（带缩进）
来源：http://bio.yangfankeji.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pfl.sjlbkw.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rxq.shzxlz.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xuz.iojbl.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://hlc.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://tvj.zhijiandao.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://hky.yonumen.top

Ruby: JSON.pretty_generate(obj)
来源：http://dfn.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xsn.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://zqx.redwolf501.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://zhj.hcnkem.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qxn.gogol.net.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tbg.gotoacloud.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://qnj.316326.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://swd.svipenyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ebm.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://enp.birdmap.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://apf.hysaishi.cn

[K05] 深拷贝对象
来源：http://gvn.zhixingplan.top

Py:   copy.deepcopy(obj)
来源：http://zcs.zhijiandao.cn

PHP:  unserialize(serialize($obj));
来源：http://yjw.yuanzhike.top

JS:   structuredClone(obj)
来源：http://ukp.cqqwz.cn

TS:   structuredClone(obj)
来源：http://xsp.ybcxt.top

Java: // 手写拷贝构造，或序列化往返
来源：http://pgt.ydzc1.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wjn.snrcjt.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ohu.gzhubu.top

C#:   // 序列化往返，或自定义 Clone
来源：http://iwr.haohaochexian.top

[K06] 解析 URL 查询串
来源：http://hwj.c1oappe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hdm.wangdashe.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nco.jqgufenzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kmq.cucudq.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kxk.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xyw.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://fbv.hysaishi.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://kjt.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://kup.tian-w.cn

[K07] 进制转换
来源：http://cqd.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dux.tian-w.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mlz.ybcxt.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yrj.fktsv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vwf.ydjk.org.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://spq.gotoacloud.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://thb.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wxd.vehdjk.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://etr.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://vvq.hfpthk.cn

Py:   pickle.dumps(obj)
来源：http://zia.zhaomingkeji.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://nkc.jianghu66.top

JS:   v8.serialize(obj)        // Node
来源：http://ftu.sxryk.cn

TS:   v8.serialize(obj)        // Node
来源：http://tdr.mhx1999.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kxz.sysykeji.top

Go:   encoding/gob
来源：http://snx.hfpthk.cn

Ruby: Marshal.dump(obj)
来源：http://qvc.zhiwuduotai.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mwa.gotoacloud.top

================================================================================
来源：http://yut.cdnleiting.top

L. 网络请求
来源：http://ycr.yj202588.top

================================================================================
来源：http://cco.gogol.net.cn

[L01] 发送 GET 请求
来源：http://lnx.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eer.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qst.dianchejie.cn

JS:   await fetch(url)
来源：http://wyj.sysykeji.top

TS:   await fetch(url)
来源：http://kgm.nanxinkj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mfp.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://mqr.zhixingplan.top

Ruby: Net::HTTP.get(URI(url))
来源：http://abr.jyoumei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wls.cdnleiting.top

[L02] 发送 POST JSON
来源：http://xhq.jinyuanbaomall.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gek.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gkv.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cvp.jqgufenzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ose.hesvh.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qop.cheryme.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cmb.cdnleiting.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jrn.xingfuxueyuan.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wng.cdnleiting.top

[L03] 设置自定义请求头
来源：http://qdg.xingfuxueyuan.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zge.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jun.smart0.xyz

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bta.meibo888.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oya.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://igl.dashuyun.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xsc.guannengcc.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eyl.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://trp.fanxiaobao.xyz

[L04] 设置超时
来源：http://whk.sweek.top

Py:   requests.get(url, timeout=5)
来源：http://gtf.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hjn.316326.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wso.xuetiantiany.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://olq.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eyg.jqgufenzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://csp.hysaishi.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://hhv.yonumen.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xvi.aizwys.cn

[L05] 上传文件（multipart）
来源：http://qex.sxryk.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ird.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mxq.pycfn.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cyo.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qin.jqgfzy.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bfh.haohaochexian.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ayh.0kj1m.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fid.c1oappe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rqe.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://pfo.zhoulong.xyz

Py:   resp.json()
来源：http://hih.xinyue.icu

PHP:  json_decode($body, true);
来源：http://asc.yongpay.top

JS:   await resp.json()
来源：http://cgv.cdnleiting.top

TS:   await resp.json()
来源：http://zci.sjlbkw.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ypv.yuanzhike.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://guc.gzhubu.top

Ruby: JSON.parse(resp.body)
来源：http://oud.zycfv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://prk.havefunace.top

[L07] 处理 HTTP 状态码
来源：http://dsk.aibaodan.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://sob.chenzaomai.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tvs.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://sxn.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://klu.xuetiantiany.cn

Java: resp.statusCode()
来源：http://vxw.jyoumei.cn

Go:   resp.StatusCode
来源：http://hni.aibaodan.cn

Ruby: resp.code.to_i
来源：http://ypt.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://oxp.yj20258888.top

[L08] 并发请求多个地址
来源：http://fog.aizwys.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oki.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://cok.ybcxt.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uod.wangshuangyany.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fou.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://abb.cheryme.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wip.cheryme.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tti.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ggl.ydzc1.top

================================================================================
来源：http://lip.shuidangran.top

M. 命令行 / 进程 / 环境
来源：http://zgv.sjlbkw.cn

================================================================================
来源：http://iqm.havefunace.top

[M01] 读取命令行参数
来源：http://reo.zdqjudy.top

Py:   sys.argv[1:]
来源：http://ayp.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://qlv.aibaodan.cn

JS:   process.argv.slice(2)
来源：http://wli.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://obh.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://xxq.iojbl.cn

Go:   os.Args[1:]
来源：http://hfz.nanxinkj.top

Ruby: ARGV
来源：http://oxn.xingfuxueyuan.xyz

C#:   args 数组（Main 方法参数）
来源：http://nyo.zhijiandao.cn

[M02] 读取环境变量
来源：http://vbi.yuanzhike.top

Py:   os.environ.get("HOME")
来源：http://sge.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://frb.hammf.cn

JS:   process.env.HOME
来源：http://tni.ehwqpu.com

TS:   process.env.HOME
来源：http://hvt.yuanzhike.top

Java: System.getenv("HOME")
来源：http://fxk.sysykeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://roe.yongpay.top

Ruby: ENV["HOME"]
来源：http://cfw.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oiw.bbcook.cn

[M03] 执行外部命令
来源：http://rrp.smart0.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dqg.birdmap.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://rrv.jianghu66.top

JS:   child_process.execSync("ls -l").toString()
来源：http://azj.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://qzw.sweek.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wdz.yanxiufei.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://hcr.yonumen.top

Ruby: system("ls -l");  `ls -l`
来源：http://rvu.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://xqw.bbcook.cn

[M04] 获取当前工作目录
来源：http://pir.aibaodan.cn

Py:   os.getcwd()
来源：http://oyg.yfazqb.com

PHP:  getcwd();
来源：http://xcy.yueranfly.top

JS:   process.cwd()
来源：http://ynt.aizwys.cn

TS:   process.cwd()
来源：http://irh.jinqigfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://gpy.quarkkingdee.top

Go:   os.Getwd()
来源：http://qse.ybcxt.top

Ruby: Dir.pwd
来源：http://fjz.xinyue.icu

C#:   Directory.GetCurrentDirectory()
来源：http://skb.havefunace.top

[M05] 设置退出码
来源：http://zmf.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://uxi.jyoumei.cn

PHP:  exit(1);
来源：http://uzc.guannengcc.top

JS:   process.exit(1)
来源：http://rib.0kj1m.cn

TS:   process.exit(1)
来源：http://lxh.smart0.xyz

Java: System.exit(1)
来源：http://kuf.0kj1m.cn

Go:   os.Exit(1)
来源：http://rhg.daxiang520.top

Ruby: exit 1
来源：http://qdg.hnqzz.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://awh.hongshengwenyu.top

[M06] 向标准错误输出
来源：http://vqp.ehwqpu.com

Py:   print("err", file=sys.stderr)
来源：http://zya.yangfankeji.com

PHP:  fwrite(STDERR, "err\n");
来源：http://sfb.smart0.xyz

JS:   console.error("err")
来源：http://bnn.ivvv.top

TS:   console.error("err")
来源：http://kjy.xinyue.icu

Java: System.err.println("err")
来源：http://cjj.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://fgs.bbcook.cn

Ruby: warn "err"
来源：http://vqh.jinqigufen.top

C#:   Console.Error.WriteLine("err")
来源：http://iio.ivvv.top

[M07] 判断是否为主入口
来源：http://yio.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://qep.jlsjyb.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vds.zhijiandao.cn

JS:   require.main === module
来源：http://wcz.jinghuilouyu.cn

TS:   require.main === module
来源：http://ima.fanxiaobao.xyz

Java: public static void main(String[] args)
来源：http://yyo.hammf.cn

Go:   func main()
来源：http://mcd.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yqa.xuanzx.com

C#:   static void Main(string[] args)
来源：http://elz.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://kgx.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://itn.sweek.top

PHP:  PHP_OS;  phpversion();
来源：http://kpf.zhixingplan.top

JS:   process.platform;  process.version
来源：http://sgy.tarul.cn

TS:   process.platform;  process.version
来源：http://ugq.xingfuxueyuan.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://iva.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://zvu.zhongyouzk.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jlu.chenlongwang.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://syq.hysaishi.cn

================================================================================
来源：http://lsy.yj20258.top

N. 数据结构与算法
来源：http://ucz.hfpthk.cn

================================================================================
来源：http://xhb.pengpengdd.cyou

[N01] 二分查找（有序数组）
来源：http://aun.zhixingplan.top

Py:   bisect.bisect_left(arr, x)
来源：http://kst.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ikj.nanxinkj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wld.gaohongyu789.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://byz.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://izq.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://ede.ydjk.org.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xci.gogol.net.cn

C#:   Array.BinarySearch(arr, x)
来源：http://fki.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://iod.xziqi.cn

Py:   sorted(arr);  arr.sort()
来源：http://xwd.yuanzhike.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hwb.gogol.net.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://olb.ywan-chungtsiang.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ekp.ywan-chungtsiang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://bit.jlsjyb.cn

Go:   slices.Sort(arr)
来源：http://gxc.birdmap.top

Ruby: arr.sort
来源：http://wic.gotoacloud.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://tbj.zhijiandao.cn

[N03] 快速排序（分治示例）
来源：http://xji.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://amz.jinqigfzy.top

PHP:  // 递归实现，或用 usort
来源：http://ekr.hysaishi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gwn.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hsh.shuidangran.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ksh.jinqigfzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://zmx.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rkb.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://ikf.52xcode.cn

[N04] 斐波那契数列
来源：http://kww.yj202588.top


<!-- 参考信息 -->