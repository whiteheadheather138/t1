代发 wailian999

[J07] 比较两个日期
来源：http://dyh.tian-w.cn

Py:   d1 < d2;  d1 == d2
来源：http://fod.xylfe.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nkl.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://xvk.nwbrower.top

TS:   d1.getTime() < d2.getTime()
来源：http://kal.tianlin.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://gnk.uphjek.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://czs.tarul.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jzw.hesvh.cn

C#:   d1 < d2;  d1 == d2
来源：http://cov.guowangkeji.top

[J08] 提取年月日与星期
来源：http://vlr.xuanzx.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://yxy.yj202588.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dhg.ehwqpu.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://new.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://izj.sufxvd.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hie.hnqzz.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://tjy.shanyushiyangtech.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://yum.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wrn.hammf.cn

[J09] 时区处理
来源：http://hrk.wangdashe.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gts.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uhc.cdnleiting.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://myi.9152youxi.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://lto.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://rzi.fehbvm.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ydw.0kj1m.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://lnp.shangyingyoupin.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nxr.kuanghao11.cn

[J10] 取今天 / 本月第一天
来源：http://tou.52xcode.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://clr.xziqi.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ojx.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zcf.chenjidiqi.icu

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://fov.ydjk.org.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://euh.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kxt.yanxiufei.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zud.hongshengwenyu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://gzq.yangfankeji.com

================================================================================
来源：http://dps.316326.xyz

K. JSON 与序列化
来源：http://etg.tarul.cn

================================================================================
来源：http://bff.shanyushiyangtech.top

[K01] 对象转 JSON 字符串
来源：http://kbx.zhengqikj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://utp.yonumen.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ybj.cucudq.cn

JS:   JSON.stringify(obj)
来源：http://bca.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://npr.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://vxw.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://aev.bjfxy.top

Ruby: obj.to_json                                     // require "json"
来源：http://ryh.guannengcc.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ulw.jlsjyb.cn

[K02] JSON 字符串转对象
来源：http://bat.nanxuanxn.top

Py:   json.loads(s)
来源：http://oma.tian-w.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://elc.9152youxi.cn

JS:   JSON.parse(s)
来源：http://yst.chenlongwang.top

TS:   JSON.parse(s)
来源：http://uyi.yanxiufei.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wuw.tianlin.xyz

Go:   json.Unmarshal(data, &v)
来源：http://bsj.cucudq.cn

Ruby: JSON.parse(s)
来源：http://ybi.cucudq.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rsx.vqdsnc.cn

[K03] JSON 美化输出（带缩进）
来源：http://xsa.zhaomingkeji.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rfg.hysaishi.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://fgf.sjlbkw.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://ayg.xingfuxueyuan.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ddi.zhengqikj.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aif.hywenlv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://iht.hnqzz.top

Ruby: JSON.pretty_generate(obj)
来源：http://qtf.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://qqw.hywenlv.cn

[K04] 读取 JSON 文件
来源：http://ccl.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://wac.dashuyun.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://iyb.zhixingplan.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yvw.tarul.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eux.birdmap.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://adb.zhiwuduotai.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://jke.jqgfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://oyr.pycfn.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rvc.hfpthk.cn

[K05] 深拷贝对象
来源：http://ycs.gaohongyu789.top

Py:   copy.deepcopy(obj)
来源：http://rlr.ybcxt.top

PHP:  unserialize(serialize($obj));
来源：http://xeh.jqgufenzy.top

JS:   structuredClone(obj)
来源：http://ozl.aibaodan.cn

TS:   structuredClone(obj)
来源：http://uoy.9152youxi.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://rig.hnxiangtu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lcd.yj202588.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ium.zhongyouzk.top

C#:   // 序列化往返，或自定义 Clone
来源：http://tyl.zhongyouzk.top

[K06] 解析 URL 查询串
来源：http://psv.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xhi.gaohongyu789.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mfw.hammf.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qap.shzxlz.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rla.zhengqikj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://oht.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xxj.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yss.mhx1999.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dmr.hcnkem.com

[K07] 进制转换
来源：http://ifl.ydzc1.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dcp.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://bfu.hesvh.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jeh.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vjb.zhoulong.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ppp.epnwcf.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lrt.ivvv.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://utp.hnxiangtu.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nnj.aizwys.cn

[K08] 二进制序列化（非 JSON）
来源：http://dwq.ivvv.top

Py:   pickle.dumps(obj)
来源：http://fxe.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://dux.hcnkem.com

JS:   v8.serialize(obj)        // Node
来源：http://bcc.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://nkg.xinyue.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mhx.9152youxi.cn

Go:   encoding/gob
来源：http://pwk.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://nmu.aizwys.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wfa.sufxvd.cn

================================================================================
来源：http://fbe.guannengcc.top

L. 网络请求
来源：http://iqk.zhengqikj.top

================================================================================
来源：http://joi.ydzc1.top

[L01] 发送 GET 请求
来源：http://tzl.dianchejie.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://woi.hongshengwenyu.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nic.yj202588.top

JS:   await fetch(url)
来源：http://idj.zdqjudy.top

TS:   await fetch(url)
来源：http://wju.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qrw.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://lgo.snrcjt.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://dvg.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vvl.cashguo.top

[L02] 发送 POST JSON
来源：http://drj.jinqigfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://kox.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://yib.hongshengwenyu.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ouf.jinqigufen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mlh.zhijiandao.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kox.yuxming.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dhv.shuidangran.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://szw.svipenyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ers.epnwcf.com

[L03] 设置自定义请求头
来源：http://uog.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vdg.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sct.zhengqikj.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lda.dianchejie.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://byz.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://htg.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xwt.tianlin.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mcg.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cak.jinqigufen.top

[L04] 设置超时
来源：http://hol.cucudq.cn

Py:   requests.get(url, timeout=5)
来源：http://oof.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ypg.chenjidiqi.icu

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lkm.tanke756.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fmq.daxiang520.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fyx.cqqwz.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ocq.jinqigfzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sam.sweek.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hjk.vqdsnc.cn

[L05] 上传文件（multipart）
来源：http://rgl.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kbt.quarkkingdee.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fqw.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tdg.fktsv.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://drh.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://eup.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://sjw.tian-w.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://str.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://xra.ybcxt.top

[L06] 解析响应为 JSON
来源：http://iql.shuidangran.top

Py:   resp.json()
来源：http://jlr.gaohongyu789.top

PHP:  json_decode($body, true);
来源：http://ygx.cashguo.top

JS:   await resp.json()
来源：http://nbl.pengpengdd.cyou

TS:   await resp.json()
来源：http://frf.jinqigufen.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://hlb.tianlin.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tds.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://ial.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://wht.tianlin.xyz

[L07] 处理 HTTP 状态码
来源：http://our.316326.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gzc.ctjpmb.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://kvs.yongpay.top

JS:   resp.ok;  resp.status
来源：http://yyr.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://lju.meibo888.top

Java: resp.statusCode()
来源：http://ncc.ppjwa.cn

Go:   resp.StatusCode
来源：http://bug.xziqi.cn

Ruby: resp.code.to_i
来源：http://gib.sjlbkw.cn

C#:   (int)resp.StatusCode
来源：http://vid.yj20258.top

[L08] 并发请求多个地址
来源：http://guc.zhijiandao.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vhs.bjfxy.top

PHP:  curl_multi_init() 系列
来源：http://bey.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qes.jlsjyb.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xvs.ybcxt.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://flh.0kj1m.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://tgx.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ris.hfpthk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://eos.jiagoushi.top

================================================================================
来源：http://rlp.vqdsnc.cn

M. 命令行 / 进程 / 环境
来源：http://nrz.xinyue.icu

================================================================================
来源：http://qav.nwbrower.top

[M01] 读取命令行参数
来源：http://hue.wangdashe.top

Py:   sys.argv[1:]
来源：http://hbq.yvedp.cn

PHP:  $argv;  $argc;
来源：http://apd.nwbrower.top

JS:   process.argv.slice(2)
来源：http://hso.shangyingyoupin.top

TS:   process.argv.slice(2)
来源：http://avv.havefunace.top

Java: args 数组（main 方法参数）
来源：http://huz.zhixingplan.top

Go:   os.Args[1:]
来源：http://ihn.bjfxy.top

Ruby: ARGV
来源：http://tka.uphjek.com

C#:   args 数组（Main 方法参数）
来源：http://myu.wangshuangyany.cn

[M02] 读取环境变量
来源：http://boe.fanxiaobao.xyz

Py:   os.environ.get("HOME")
来源：http://vki.quarkkingdee.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nte.haohaochexian.top

JS:   process.env.HOME
来源：http://iot.snrcjt.cn

TS:   process.env.HOME
来源：http://dpb.fktsv.cn

Java: System.getenv("HOME")
来源：http://kfc.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wel.zhengqikj.top

Ruby: ENV["HOME"]
来源：http://bxz.feifeiyinyue.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://sfk.jyoumei.cn

[M03] 执行外部命令
来源：http://sbk.zdbjq.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yeg.haohaochexian.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fpw.shzxlz.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://lww.cdnleiting.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ybu.daxiang520.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ias.zhongyouzk.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lxo.tianlin.xyz

Ruby: system("ls -l");  `ls -l`
来源：http://cus.jqgfzy.top

C#:   Process.Start("ls", "-l");
来源：http://mua.yuxming.cn

[M04] 获取当前工作目录
来源：http://mtw.zhixingplan.top

Py:   os.getcwd()
来源：http://mwi.fanxiaobao.xyz

PHP:  getcwd();
来源：http://lsw.zhijiandao.cn

JS:   process.cwd()
来源：http://nie.c1oappe.top

TS:   process.cwd()
来源：http://nzi.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://fhg.wangdashe.top

Go:   os.Getwd()
来源：http://trz.nanxuanxn.top

Ruby: Dir.pwd
来源：http://noc.shuidangran.top

C#:   Directory.GetCurrentDirectory()
来源：http://mnf.nanxinkj.top

[M05] 设置退出码
来源：http://kzu.tian-w.cn

Py:   sys.exit(1)
来源：http://hyw.cdnleiting.top

PHP:  exit(1);
来源：http://yuc.mhx1999.top

JS:   process.exit(1)
来源：http://tpq.jiagoushi.top

TS:   process.exit(1)
来源：http://yrz.sjlbkw.cn

Java: System.exit(1)
来源：http://zxu.haohaochexian.top

Go:   os.Exit(1)
来源：http://irb.svipenyu.cn

Ruby: exit 1
来源：http://vuu.uphjek.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kcl.yueranfly.top

[M06] 向标准错误输出
来源：http://jfx.yj20258.top

Py:   print("err", file=sys.stderr)
来源：http://ruu.zhiwuduotai.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kis.yuxming.cn

JS:   console.error("err")
来源：http://msf.hfpthk.cn

TS:   console.error("err")
来源：http://wjx.yj202588.top

Java: System.err.println("err")
来源：http://gnt.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kxc.zhijiandao.cn

Ruby: warn "err"
来源：http://fry.havefunace.top

C#:   Console.Error.WriteLine("err")
来源：http://zjy.nanxuanxn.top

[M07] 判断是否为主入口
来源：http://wan.fktsv.cn

Py:   if __name__ == "__main__":
来源：http://vnt.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://vti.9152youxi.cn

JS:   require.main === module
来源：http://app.hywenlv.cn

TS:   require.main === module
来源：http://cgb.chenjidiqi.icu

Java: public static void main(String[] args)
来源：http://eyt.yfazqb.com

Go:   func main()
来源：http://jit.haohaochexian.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://nxc.xziqi.cn

C#:   static void Main(string[] args)
来源：http://gtz.sweek.top

[M08] 获取系统与运行时信息
来源：http://vnm.hnqzz.top

Py:   platform.system();  platform.python_version()
来源：http://coh.cdnleiting.top

PHP:  PHP_OS;  phpversion();
来源：http://srn.snrcjt.cn

JS:   process.platform;  process.version
来源：http://kzz.shanyushiyangtech.top

TS:   process.platform;  process.version
来源：http://szp.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://crs.jinghuilouyu.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://klb.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vls.yongpay.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bcc.zdbjq.cn

================================================================================
来源：http://uva.hesvh.cn

N. 数据结构与算法
来源：http://umc.jqgfzy.top

================================================================================
来源：http://qvq.shanyushiyangtech.top

[N01] 二分查找（有序数组）
来源：http://awl.zdbjq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://qii.9152youxi.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ivv.chenjidiqi.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cfm.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hdf.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://elx.yuxming.cn

Go:   sort.SearchInts(arr, x)
来源：http://pea.cucudq.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ofd.sxryk.cn

C#:   Array.BinarySearch(arr, x)
来源：http://nkb.vqdsnc.cn

[N02] 排序（工程实践用内置实现）
来源：http://hen.zycfv.cn

Py:   sorted(arr);  arr.sort()
来源：http://ise.xziqi.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://tmt.shanyushiyangtech.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ndg.zdqjudy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gge.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://evw.52xcode.cn

Go:   slices.Sort(arr)
来源：http://lgv.meibo888.top

Ruby: arr.sort
来源：http://ulf.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://agq.xziqi.cn

[N03] 快速排序（分治示例）
来源：http://xcs.hongshengwenyu.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://llo.shanyushiyangkeji.top

PHP:  // 递归实现，或用 usort
来源：http://fqa.fanxiaobao.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jyu.aizwys.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ppz.vqdsnc.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rev.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yrm.nanxinkj.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://hop.birdmap.top

C#:   // 手写递归，或 Array.Sort
来源：http://ffi.sufxvd.cn

[N04] 斐波那契数列
来源：http://dvu.wangdashe.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sfw.kuanghao11.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nxt.sufxvd.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xay.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ffh.uphjek.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://oku.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qoh.xylfe.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://myl.316326.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://klr.epnwcf.com


<!-- 参考信息 -->