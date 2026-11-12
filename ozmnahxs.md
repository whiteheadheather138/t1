代发 wailian999

[J07] 比较两个日期
来源：http://wbg.kuanghao11.cn

Py:   d1 < d2;  d1 == d2
来源：http://nvl.tian-w.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://vus.meibo888.top

JS:   d1.getTime() < d2.getTime()
来源：http://cwg.jyoumei.cn

TS:   d1.getTime() < d2.getTime()
来源：http://out.yueranfly.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nlu.ppjwa.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://vgi.xinyue.icu

Ruby: d1 < d2;  d1 == d2
来源：http://myi.fanxiaobao.xyz

C#:   d1 < d2;  d1 == d2
来源：http://sbh.jyoumei.cn

[J08] 提取年月日与星期
来源：http://kkn.tarul.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://rcc.gotoacloud.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ebr.c1oappe.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://yxt.gzhubu.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://noq.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://tem.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://hnr.xuanzx.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://rqi.hfpthk.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://arx.sjlbkw.cn

[J09] 时区处理
来源：http://hay.ydjk.org.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://mkt.feifeiyinyue.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://ovu.nwbrower.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fuf.jqgufenzy.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://frm.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wro.zycfv.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://wov.snrcjt.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://wzf.yj202588.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fdb.jinghuilouyu.cn

[J10] 取今天 / 本月第一天
来源：http://inr.ehwqpu.com

Py:   date.today();  date.today().replace(day=1)
来源：http://bef.hnqzz.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://yxg.nanxinkj.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ask.xinyue.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uvt.xylfe.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://gnw.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ayq.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bav.fanxiaobao.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eqe.tarul.cn

================================================================================
来源：http://mmk.ybcxt.top

K. JSON 与序列化
来源：http://pcx.tarul.cn

================================================================================
来源：http://bsy.shanyushiyangkeji.top

[K01] 对象转 JSON 字符串
来源：http://bax.mhx1999.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lob.hammf.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rtx.guannengcc.top

JS:   JSON.stringify(obj)
来源：http://hjp.iojbl.cn

TS:   JSON.stringify(obj)
来源：http://udn.xuanzx.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://nhh.chenzaomai.com

Go:   json.Marshal(obj)
来源：http://lqn.tian-w.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mpb.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://smh.jqgfzy.top

[K02] JSON 字符串转对象
来源：http://fvl.hongshengwenyu.top

Py:   json.loads(s)
来源：http://vkg.zhengqikj.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jpa.0kj1m.cn

JS:   JSON.parse(s)
来源：http://hlp.ybcxt.top

TS:   JSON.parse(s)
来源：http://xli.cucudq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vgz.sxryk.cn

Go:   json.Unmarshal(data, &v)
来源：http://eww.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://glk.vqdsnc.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dym.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://qax.c1oappe.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://llb.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kvn.birdmap.top

JS:   JSON.stringify(obj, null, 2)
来源：http://qdi.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://jbc.gotoacloud.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://set.daria6918.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://vbg.guowangkeji.top

Ruby: JSON.pretty_generate(obj)
来源：http://jlj.meibo888.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://brs.jiagoushi.top

[K04] 读取 JSON 文件
来源：http://zqr.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://chl.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iju.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lbs.quarkkingdee.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://unf.feifeiyinyue.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://nll.xinyue.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xgj.uphjek.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://gel.ywan-chungtsiang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://zku.xylfe.cn

[K05] 深拷贝对象
来源：http://qbl.hammf.cn

Py:   copy.deepcopy(obj)
来源：http://mqy.yfazqb.com

PHP:  unserialize(serialize($obj));
来源：http://opt.jinqigufen.top

JS:   structuredClone(obj)
来源：http://dko.yuxming.cn

TS:   structuredClone(obj)
来源：http://dee.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://jcc.xylfe.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://oeg.hfpthk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://afm.ivvv.top

C#:   // 序列化往返，或自定义 Clone
来源：http://bdt.yangfankeji.com

[K06] 解析 URL 查询串
来源：http://der.hnqzz.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://noe.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vwl.fengsongda.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gwe.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://onv.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ufw.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://oby.c1oappe.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://jec.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yrv.shuidangran.top

[K07] 进制转换
来源：http://gkf.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dsz.yueranfly.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://fsm.vqdsnc.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://asd.svipenyu.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://gbj.epnwcf.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://sie.yonumen.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://blp.52xcode.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ude.daxiang520.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jec.aibaodan.cn

[K08] 二进制序列化（非 JSON）
来源：http://sdb.ydzc1.top

Py:   pickle.dumps(obj)
来源：http://obj.hywenlv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://wlx.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://bri.jqgufenzy.top

TS:   v8.serialize(obj)        // Node
来源：http://nbi.fehbvm.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://rbn.ivvv.top

Go:   encoding/gob
来源：http://wpv.wangshuangyany.cn

Ruby: Marshal.dump(obj)
来源：http://xcf.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kbk.guannengcc.top

================================================================================
来源：http://erb.cucudq.cn

L. 网络请求
来源：http://yuz.yj202588.top

================================================================================
来源：http://ppk.fehbvm.com

[L01] 发送 GET 请求
来源：http://qeg.ppjwa.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qtu.guannengcc.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tpm.chenlongwang.top

JS:   await fetch(url)
来源：http://chn.zycfv.cn

TS:   await fetch(url)
来源：http://jat.sjlbkw.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hzx.fengsongda.top

Go:   resp, err := http.Get(url)
来源：http://chs.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://joq.cdnleiting.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://scg.daxiang520.top

[L02] 发送 POST JSON
来源：http://kgr.hnxiangtu.top

Py:   requests.post(url, json={"a": 1})
来源：http://zpt.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vzb.sjlbkw.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qlb.vehdjk.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kxb.316326.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tis.andypj.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ifu.316326.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://oie.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fok.feifeiyinyue.top

[L03] 设置自定义请求头
来源：http://sav.shanyushiyangtech.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://awj.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hsw.ydjk.org.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pva.mhx1999.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ewn.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://tbi.yangfankeji.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://kbu.hesvh.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://vrg.yonumen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dpq.mhx1999.top

[L04] 设置超时
来源：http://ulp.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://hdf.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://icg.gotoacloud.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oom.jinqigfzy.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://oew.bjfxy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wra.hammf.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zve.hcnkem.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ara.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://upn.c1oappe.top

[L05] 上传文件（multipart）
来源：http://ikb.cucudq.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://emk.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://pgn.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://cwq.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://wpk.feifeiyinyue.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xqu.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://pdt.vehdjk.com

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://tpa.yongpay.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jwt.shanyushiyangkeji.top

[L06] 解析响应为 JSON
来源：http://fjl.jianghu66.top

Py:   resp.json()
来源：http://hsq.feifeiyinyue.top

PHP:  json_decode($body, true);
来源：http://xgn.zhongyouzk.top

JS:   await resp.json()
来源：http://fbb.tanke756.top

TS:   await resp.json()
来源：http://dio.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ipv.c1oappe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://rri.kuanghao11.cn

Ruby: JSON.parse(resp.body)
来源：http://mic.sysykeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jpu.snrcjt.cn

[L07] 处理 HTTP 状态码
来源：http://uvv.hnqzz.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qwv.hesvh.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://tcp.sjlbkw.cn

JS:   resp.ok;  resp.status
来源：http://xrx.cashguo.top

TS:   resp.ok;  resp.status
来源：http://exs.meibo888.top

Java: resp.statusCode()
来源：http://tsj.yuxming.cn

Go:   resp.StatusCode
来源：http://miw.iojbl.cn

Ruby: resp.code.to_i
来源：http://nod.cucudq.cn

C#:   (int)resp.StatusCode
来源：http://piq.svipenyu.cn

[L08] 并发请求多个地址
来源：http://whi.daria6918.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://wll.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://vwn.nanxuanxn.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ffj.pengpengdd.cyou

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://asw.uphjek.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vnp.snrcjt.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qye.cucudq.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uvm.pycfn.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ans.redwolf501.top

================================================================================
来源：http://pom.cashguo.top

M. 命令行 / 进程 / 环境
来源：http://cgz.tanke756.top

================================================================================
来源：http://sqz.bbcook.cn

[M01] 读取命令行参数
来源：http://fdb.shuidangran.top

Py:   sys.argv[1:]
来源：http://gos.sufxvd.cn

PHP:  $argv;  $argc;
来源：http://wik.redwolf501.top

JS:   process.argv.slice(2)
来源：http://ilx.sufxvd.cn

TS:   process.argv.slice(2)
来源：http://rtl.fengsongda.top

Java: args 数组（main 方法参数）
来源：http://cgr.svipenyu.cn

Go:   os.Args[1:]
来源：http://fwd.pycfn.com

Ruby: ARGV
来源：http://boj.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://ifk.yueranfly.top

[M02] 读取环境变量
来源：http://tos.aizwys.cn

Py:   os.environ.get("HOME")
来源：http://ojg.xingfuxueyuan.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://deu.zhiwuduotai.top

JS:   process.env.HOME
来源：http://akm.ppjwa.cn

TS:   process.env.HOME
来源：http://nve.fengsongda.top

Java: System.getenv("HOME")
来源：http://qnw.yj202588.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tie.zycfv.cn

Ruby: ENV["HOME"]
来源：http://nvd.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dgi.quarkkingdee.top

[M03] 执行外部命令
来源：http://nhe.guannengcc.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://maf.nwbrower.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ivl.ppjwa.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://cxq.sysykeji.top

TS:   child_process.execSync("ls -l").toString()
来源：http://abj.zhengqikj.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xwm.9152youxi.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://veo.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://uab.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://pkq.ctjpmb.com

[M04] 获取当前工作目录
来源：http://fyb.jinqigfzy.top

Py:   os.getcwd()
来源：http://npf.mhx1999.top

PHP:  getcwd();
来源：http://keg.zhijiandao.cn

JS:   process.cwd()
来源：http://gvx.gaohongyu789.top

TS:   process.cwd()
来源：http://idu.hesvh.cn

Java: Path.of("").toAbsolutePath()
来源：http://iqx.tanke756.top

Go:   os.Getwd()
来源：http://cxz.yuanzhike.top

Ruby: Dir.pwd
来源：http://pqs.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://sbj.jlsjyb.cn

[M05] 设置退出码
来源：http://yys.zhoulong.xyz

Py:   sys.exit(1)
来源：http://ewb.ivvv.top

PHP:  exit(1);
来源：http://fca.jinyuanbaomall.cn

JS:   process.exit(1)
来源：http://dps.yanxiufei.cn

TS:   process.exit(1)
来源：http://gkx.birdmap.top

Java: System.exit(1)
来源：http://zsn.yueranfly.top

Go:   os.Exit(1)
来源：http://mlz.cheryme.top

Ruby: exit 1
来源：http://egf.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bla.quarkkingdee.top

[M06] 向标准错误输出
来源：http://org.yueranfly.top

Py:   print("err", file=sys.stderr)
来源：http://rnv.tarul.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://wep.aizwys.cn

JS:   console.error("err")
来源：http://teb.ctjpmb.com

TS:   console.error("err")
来源：http://ouu.fehbvm.com

Java: System.err.println("err")
来源：http://has.jiagoushi.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hfa.zhijiandao.cn

Ruby: warn "err"
来源：http://vpy.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://bry.wangdashe.top

[M07] 判断是否为主入口
来源：http://byj.gogol.net.cn

Py:   if __name__ == "__main__":
来源：http://czc.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lzo.tanke756.top

JS:   require.main === module
来源：http://rih.hnqzz.top

TS:   require.main === module
来源：http://ysh.nwbrower.top

Java: public static void main(String[] args)
来源：http://hsr.jiagoushi.top

Go:   func main()
来源：http://skm.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rtz.tianlin.xyz

C#:   static void Main(string[] args)
来源：http://sxs.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://dse.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://dlh.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://ptz.vehdjk.com

JS:   process.platform;  process.version
来源：http://bdx.sweek.top

TS:   process.platform;  process.version
来源：http://vfj.cashguo.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://slt.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://vrf.daxiang520.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://aic.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://gop.fktsv.cn

================================================================================
来源：http://wyg.shanyushiyangkeji.top

N. 数据结构与算法
来源：http://ufu.guowangkeji.top

================================================================================
来源：http://bqe.hnqzz.top

[N01] 二分查找（有序数组）
来源：http://tqq.cheryme.top

Py:   bisect.bisect_left(arr, x)
来源：http://ytr.ybcxt.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tcg.aizwys.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vpb.gotoacloud.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zgr.mhx1999.top

Java: Arrays.binarySearch(arr, x)
来源：http://mng.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://qiy.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ckz.xingfuxueyuan.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://xoe.jianghu66.top

[N02] 排序（工程实践用内置实现）
来源：http://lmc.tanke756.top

Py:   sorted(arr);  arr.sort()
来源：http://xyu.c1oappe.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tti.shanyushiyangkeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vfs.jlsjyb.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rrl.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://twq.zhixingplan.top

Go:   slices.Sort(arr)
来源：http://dzh.bjfxy.top

Ruby: arr.sort
来源：http://tvc.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://ywn.cqqwz.cn

[N03] 快速排序（分治示例）
来源：http://gux.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ice.sysykeji.top

PHP:  // 递归实现，或用 usort
来源：http://oyj.xuanzx.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wja.zhongyouzk.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://eiy.shangyingyoupin.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wve.jiagoushi.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qor.fengsongda.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nxp.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://ifj.yvedp.cn

[N04] 斐波那契数列
来源：http://lvp.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xru.gaohongyu789.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://iyp.svipenyu.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://heb.kuanghao11.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ztx.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dhy.xinyue.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://oge.wangdashe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fof.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vjo.birdmap.top


<!-- 参考信息 -->