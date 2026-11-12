代发 wailian999

Go:   time.Now().AddDate(0, 0, 7)
来源：http://oxv.haohaochexian.top

Ruby: Time.now + 7 * 86400
来源：http://pyo.zhoulong.xyz

C#:   DateTime.Now.AddDays(7)
来源：http://sbt.andypj.xyz

[J06] 计算两时间之差
来源：http://myl.zhoulong.xyz

Py:   (end - start).total_seconds()
来源：http://xwz.hfpthk.cn

PHP:  $end->diff($start)->days;
来源：http://yqt.hfpthk.cn

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://bqr.shanyushiyangtech.top

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://wfp.andypj.xyz

Java: Duration.between(start, end).toSeconds()
来源：http://tyq.zhoulong.xyz

Go:   end.Sub(start).Hours()
来源：http://eoj.52xcode.cn

Ruby: end - start                 # 返回秒数
来源：http://vqo.mhx1999.top

C#:   (end - start).TotalSeconds
来源：http://vzc.uphjek.com

[J07] 比较两个日期
来源：http://vep.vqdsnc.cn

Py:   d1 < d2;  d1 == d2
来源：http://qsu.pycfn.com

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://tjs.jinghuilouyu.cn

JS:   d1.getTime() < d2.getTime()
来源：http://rks.gzhubu.top

TS:   d1.getTime() < d2.getTime()
来源：http://mqd.tian-w.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://bdb.tarul.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://gts.sjlbkw.cn

Ruby: d1 < d2;  d1 == d2
来源：http://wgc.chenlongwang.top

C#:   d1 < d2;  d1 == d2
来源：http://znb.hammf.cn

[J08] 提取年月日与星期
来源：http://hmt.epnwcf.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lkf.nanxinkj.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ddw.andypj.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rim.sufxvd.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xqb.daria6918.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dhf.zhengqikj.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://cvr.nanxinkj.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fmq.yangfankeji.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ufp.bjfxy.top

[J09] 时区处理
来源：http://blw.yueranfly.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://dsr.sweek.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rwz.daxiang520.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ogz.chenjidiqi.icu

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ipk.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wqv.nwbrower.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://fpu.ivvv.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fqx.yanxiufei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://gzn.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://xch.bbcook.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://cor.tanke756.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://pqm.quarkkingdee.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://gvy.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://osh.tian-w.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gvk.xinyue.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://itq.shangyingyoupin.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://oxn.epnwcf.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dwn.sjlbkw.cn

================================================================================
来源：http://aes.yj202588.top

K. JSON 与序列化
来源：http://dar.aizwys.cn

================================================================================
来源：http://dsz.jinyuanbaomall.cn

[K01] 对象转 JSON 字符串
来源：http://jyj.jqgfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://raa.zdqjudy.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cah.nanxinkj.top

JS:   JSON.stringify(obj)
来源：http://xxu.sxryk.cn

TS:   JSON.stringify(obj)
来源：http://znq.andypj.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cvt.yangfankeji.com

Go:   json.Marshal(obj)
来源：http://ybo.hcnkem.com

Ruby: obj.to_json                                     // require "json"
来源：http://kik.fanxiaobao.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://nax.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://dqu.kuanghao11.cn

Py:   json.loads(s)
来源：http://ffl.tanke756.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mkf.shanyushiyangtech.top

JS:   JSON.parse(s)
来源：http://aqh.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://ekx.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ion.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://okp.aizwys.cn

Ruby: JSON.parse(s)
来源：http://zgo.xuetiantiany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lcz.yuanzhike.top

[K03] JSON 美化输出（带缩进）
来源：http://wyn.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://eqx.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fav.jinqigfzy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wvt.pengpengdd.cyou

TS:   JSON.stringify(obj, null, 2)
来源：http://wko.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://due.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fzs.shanyushiyangtech.top

Ruby: JSON.pretty_generate(obj)
来源：http://spu.cheryme.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://wxb.mhx1999.top

[K04] 读取 JSON 文件
来源：http://vng.0kj1m.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rgl.daria6918.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://pwi.kuanghao11.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://byf.pengpengdd.cyou

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ggy.yueranfly.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ese.jyoumei.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jae.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rjl.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://esn.ybcxt.top

[K05] 深拷贝对象
来源：http://jza.yuxming.cn

Py:   copy.deepcopy(obj)
来源：http://msl.ydjk.org.cn

PHP:  unserialize(serialize($obj));
来源：http://whv.andypj.xyz

JS:   structuredClone(obj)
来源：http://jhw.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://yuk.fanxiaobao.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://vwy.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://izp.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://xid.yvedp.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://uri.hcnkem.com

[K06] 解析 URL 查询串
来源：http://osy.gogol.net.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://vlh.yuxming.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uaz.jiagoushi.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ful.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rbc.yj20258888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zau.ivvv.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://qbp.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xxi.birdmap.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bil.fanxiaobao.xyz

[K07] 进制转换
来源：http://gyy.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gzn.bjfxy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ezd.shanyushiyangkeji.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zfh.ivvv.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fua.yonumen.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://upx.zhixingplan.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://srt.tianlin.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hqa.svipenyu.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ocz.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://efa.daxiang520.top

Py:   pickle.dumps(obj)
来源：http://xel.andypj.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ocf.zhiwuduotai.top

JS:   v8.serialize(obj)        // Node
来源：http://utf.hnxiangtu.top

TS:   v8.serialize(obj)        // Node
来源：http://wjk.fzhhl.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uws.fktsv.cn

Go:   encoding/gob
来源：http://oma.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://xde.c1oappe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aqt.yuxming.cn

================================================================================
来源：http://afh.nanxinkj.top

L. 网络请求
来源：http://lss.zhaomingkeji.xyz

================================================================================
来源：http://pcv.hysaishi.cn

[L01] 发送 GET 请求
来源：http://xvm.svipenyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dhw.yuxming.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pdb.fehbvm.com

JS:   await fetch(url)
来源：http://xfd.sjlbkw.cn

TS:   await fetch(url)
来源：http://cir.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://mmk.zhoulong.xyz

Go:   resp, err := http.Get(url)
来源：http://xbt.dashuyun.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://pir.shzxlz.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ity.yj202588.top

[L02] 发送 POST JSON
来源：http://qmq.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://ayj.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zco.52xcode.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jpn.gogol.net.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qfo.yj20258.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aje.cashguo.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jdu.daria6918.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://zrg.yj202588.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rfk.vqdsnc.cn

[L03] 设置自定义请求头
来源：http://xvs.dianchejie.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://flk.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vlo.svipenyu.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://els.andypj.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xgs.snrcjt.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mhv.zycfv.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sob.epnwcf.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ieo.zhaomingkeji.xyz

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yfv.yongpay.top

[L04] 设置超时
来源：http://ofu.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://fze.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ode.yanxiufei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zwo.cashguo.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uwi.9152youxi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rsf.hcnkem.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://huu.ywan-chungtsiang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://trc.yangfankeji.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://buv.sjlbkw.cn

[L05] 上传文件（multipart）
来源：http://xct.chenzaomai.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zkb.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tmo.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cwv.andypj.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jxm.fzhhl.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kuc.sxryk.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dwh.bjfxy.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://huo.daria6918.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hez.xuetiantiany.cn

[L06] 解析响应为 JSON
来源：http://kyv.hnqzz.top

Py:   resp.json()
来源：http://izs.jqgufenzy.top

PHP:  json_decode($body, true);
来源：http://tcs.vehdjk.com

JS:   await resp.json()
来源：http://joi.cashguo.top

TS:   await resp.json()
来源：http://gfr.daria6918.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kzo.ybcxt.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://dvu.redwolf501.top

Ruby: JSON.parse(resp.body)
来源：http://khm.jyoumei.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://gue.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://giq.jqgufenzy.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ngt.yvedp.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qsy.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://zoj.yj20258.top

TS:   resp.ok;  resp.status
来源：http://gac.fzhhl.top

Java: resp.statusCode()
来源：http://exb.zhijiandao.cn

Go:   resp.StatusCode
来源：http://rpq.bbcook.cn

Ruby: resp.code.to_i
来源：http://sdd.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://rle.zhijiandao.cn

[L08] 并发请求多个地址
来源：http://svg.bjfxy.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sya.zhoulong.xyz

PHP:  curl_multi_init() 系列
来源：http://ewd.feifeiyinyue.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://avg.epnwcf.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://sip.feifeiyinyue.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yja.zhijiandao.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wii.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qpz.hongshengwenyu.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://slw.haohaochexian.top

================================================================================
来源：http://spg.ydzc1.top

M. 命令行 / 进程 / 环境
来源：http://tmi.316326.xyz

================================================================================
来源：http://cmc.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://cvm.shzxlz.cn

Py:   sys.argv[1:]
来源：http://uxj.yfazqb.com

PHP:  $argv;  $argc;
来源：http://yrn.chenlongwang.top

JS:   process.argv.slice(2)
来源：http://dbs.ivvv.top

TS:   process.argv.slice(2)
来源：http://dri.jinghuilouyu.cn

Java: args 数组（main 方法参数）
来源：http://mnp.hnxiangtu.top

Go:   os.Args[1:]
来源：http://vng.ydjk.org.cn

Ruby: ARGV
来源：http://yow.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://qcb.yuxming.cn

[M02] 读取环境变量
来源：http://wio.yueranfly.top

Py:   os.environ.get("HOME")
来源：http://man.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://aqg.jinghuilouyu.cn

JS:   process.env.HOME
来源：http://zrl.jyoumei.cn

TS:   process.env.HOME
来源：http://fck.birdmap.top

Java: System.getenv("HOME")
来源：http://gnf.yuxming.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ioe.xingfuxueyuan.xyz

Ruby: ENV["HOME"]
来源：http://zsc.smart0.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hnk.mhx1999.top

[M03] 执行外部命令
来源：http://qlp.zycfv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nwh.ppjwa.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cgt.tianlin.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://ibr.chenzaomai.com

TS:   child_process.execSync("ls -l").toString()
来源：http://mxk.9152youxi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ntk.sysykeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ckh.mhx1999.top

Ruby: system("ls -l");  `ls -l`
来源：http://crw.svipenyu.cn

C#:   Process.Start("ls", "-l");
来源：http://ekh.yj20258.top

[M04] 获取当前工作目录
来源：http://nfm.hywenlv.cn

Py:   os.getcwd()
来源：http://gvq.fktsv.cn

PHP:  getcwd();
来源：http://uzh.sjlbkw.cn

JS:   process.cwd()
来源：http://nwg.hnqzz.top

TS:   process.cwd()
来源：http://qag.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://etm.xuanzx.com

Go:   os.Getwd()
来源：http://vxw.zhixingplan.top

Ruby: Dir.pwd
来源：http://ajb.hammf.cn

C#:   Directory.GetCurrentDirectory()
来源：http://eoi.hysaishi.cn

[M05] 设置退出码
来源：http://yic.wangdashe.top

Py:   sys.exit(1)
来源：http://wvj.jyoumei.cn

PHP:  exit(1);
来源：http://myt.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://vqo.yonumen.top

TS:   process.exit(1)
来源：http://tzd.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://yit.nwbrower.top

Go:   os.Exit(1)
来源：http://req.yonumen.top

Ruby: exit 1
来源：http://gje.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://chs.nwbrower.top

[M06] 向标准错误输出
来源：http://lxt.dashuyun.cn

Py:   print("err", file=sys.stderr)
来源：http://dlu.cqqwz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tzr.yj20258.top

JS:   console.error("err")
来源：http://dvu.gaohongyu789.top

TS:   console.error("err")
来源：http://zfz.chenlongwang.top

Java: System.err.println("err")
来源：http://ohi.zhongyouzk.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pif.gogol.net.cn

Ruby: warn "err"
来源：http://swo.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://dbp.fktsv.cn

[M07] 判断是否为主入口
来源：http://led.yanxiufei.cn

Py:   if __name__ == "__main__":
来源：http://iej.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://dgw.ywan-chungtsiang.top

JS:   require.main === module
来源：http://hxn.ybcxt.top

TS:   require.main === module
来源：http://wgy.cashguo.top

Java: public static void main(String[] args)
来源：http://voc.nanxinkj.top

Go:   func main()
来源：http://tlg.chenjidiqi.icu

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://spo.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://wgo.gotoacloud.top

[M08] 获取系统与运行时信息
来源：http://yfm.svipenyu.cn

Py:   platform.system();  platform.python_version()
来源：http://zys.fktsv.cn

PHP:  PHP_OS;  phpversion();
来源：http://ovc.zdqjudy.top

JS:   process.platform;  process.version
来源：http://xtn.kuanghao11.cn

TS:   process.platform;  process.version
来源：http://pnf.andypj.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://vue.tianlin.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://jcj.gogol.net.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tkb.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://hqg.haohaochexian.top

================================================================================
来源：http://fde.yj202588.top

N. 数据结构与算法
来源：http://nol.jinqigufen.top

================================================================================
来源：http://hig.wangshuangyany.cn

[N01] 二分查找（有序数组）
来源：http://jwp.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://pse.shanyushiyangkeji.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tzi.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ish.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uzt.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lib.yongpay.top

Go:   sort.SearchInts(arr, x)
来源：http://pqc.hcnkem.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://zmz.fehbvm.com

C#:   Array.BinarySearch(arr, x)
来源：http://fxa.jinqigufen.top

[N02] 排序（工程实践用内置实现）
来源：http://ahp.ehwqpu.com

Py:   sorted(arr);  arr.sort()
来源：http://ysp.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bfx.tarul.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://lrr.redwolf501.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://uxg.bbcook.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://muo.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://yfm.hnqzz.top

Ruby: arr.sort
来源：http://puk.yj20258.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pec.tarul.cn

[N03] 快速排序（分治示例）
来源：http://zcn.nanxinkj.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qbn.nwbrower.top

PHP:  // 递归实现，或用 usort
来源：http://ijb.gaohongyu789.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kgv.pengpengdd.cyou

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gjl.havefunace.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vtx.yfazqb.com


<!-- 参考信息 -->