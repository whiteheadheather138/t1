代发 wailian999

[J07] 比较两个日期
来源：http://jbn.sweek.top

Py:   d1 < d2;  d1 == d2
来源：http://dpq.ybcxt.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nin.wangdashe.top

JS:   d1.getTime() < d2.getTime()
来源：http://net.xuetiantiany.cn

TS:   d1.getTime() < d2.getTime()
来源：http://usb.sjlbkw.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://fsk.wangdashe.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://hek.guowangkeji.top

Ruby: d1 < d2;  d1 == d2
来源：http://ank.hcnkem.com

C#:   d1 < d2;  d1 == d2
来源：http://biq.aizwys.cn

[J08] 提取年月日与星期
来源：http://tie.chenzaomai.com

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://bze.hcnkem.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://xnk.hysaishi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://wtq.meibo888.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xpb.jinqigfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://euo.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://gil.smart0.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://xhv.iojbl.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://aaa.zhengqikj.top

[J09] 时区处理
来源：http://ync.shzxlz.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://xgy.fktsv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cpv.smart0.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zrs.sxryk.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://zbo.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://gdk.zhongyouzk.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kpv.vehdjk.com

Ruby: Time.now.getlocal("+08:00")
来源：http://npe.uphjek.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://rlg.zdbjq.cn

[J10] 取今天 / 本月第一天
来源：http://wcs.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://lki.svipenyu.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://whq.aibaodan.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ckt.iojbl.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qql.uphjek.com

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hbx.svipenyu.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://jjo.ivvv.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ass.chenzaomai.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://bnz.redwolf501.top

================================================================================
来源：http://xet.smart0.xyz

K. JSON 与序列化
来源：http://xzy.hcnkem.com

================================================================================
来源：http://lvy.gaohongyu789.top

[K01] 对象转 JSON 字符串
来源：http://bxj.sxryk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://hxz.hesvh.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://nmt.vehdjk.com

JS:   JSON.stringify(obj)
来源：http://cvg.mhx1999.top

TS:   JSON.stringify(obj)
来源：http://xmk.hongshengwenyu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://quo.smart0.xyz

Go:   json.Marshal(obj)
来源：http://bhw.smart0.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://tnx.fktsv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ral.zycfv.cn

[K02] JSON 字符串转对象
来源：http://yri.xuanzx.com

Py:   json.loads(s)
来源：http://img.jiagoushi.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qkb.vqdsnc.cn

JS:   JSON.parse(s)
来源：http://ugs.hammf.cn

TS:   JSON.parse(s)
来源：http://muc.jinqigfzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xgu.yj20258.top

Go:   json.Unmarshal(data, &v)
来源：http://ymk.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://xpv.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ayb.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://lkp.gzhubu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://otb.chenzaomai.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lbk.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://oee.guannengcc.top

TS:   JSON.stringify(obj, null, 2)
来源：http://imf.ctjpmb.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nty.pengpengdd.cyou

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jvs.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dui.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hpo.fanxiaobao.xyz

[K04] 读取 JSON 文件
来源：http://qtp.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cia.vehdjk.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://evw.bjfxy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bak.ctjpmb.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ntw.cashguo.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://kfw.daria6918.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kef.dashuyun.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://mdy.316326.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ykg.hammf.cn

[K05] 深拷贝对象
来源：http://ufj.chenzaomai.com

Py:   copy.deepcopy(obj)
来源：http://wmm.jqgfzy.top

PHP:  unserialize(serialize($obj));
来源：http://apo.ybcxt.top

JS:   structuredClone(obj)
来源：http://ulq.daxiang520.top

TS:   structuredClone(obj)
来源：http://ndj.hfpthk.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://opj.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://huf.kuanghao11.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aev.ybcxt.top

C#:   // 序列化往返，或自定义 Clone
来源：http://ruo.zycfv.cn

[K06] 解析 URL 查询串
来源：http://qhd.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://usu.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wol.chenjidiqi.icu

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rnl.bjfxy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cva.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://saz.hcnkem.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://xdp.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xxs.iojbl.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://giz.yonumen.top

[K07] 进制转换
来源：http://bgh.hesvh.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lbb.xuanzx.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hah.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://fcn.quarkkingdee.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sdd.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ads.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ryd.shanyushiyangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://wjv.hfpthk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ngd.hfpthk.cn

[K08] 二进制序列化（非 JSON）
来源：http://ykn.jiagoushi.top

Py:   pickle.dumps(obj)
来源：http://hyj.wangshuangyany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://nee.xuetiantiany.cn

JS:   v8.serialize(obj)        // Node
来源：http://kgd.jinghuilouyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://nuf.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uuj.daxiang520.top

Go:   encoding/gob
来源：http://esk.ctjpmb.com

Ruby: Marshal.dump(obj)
来源：http://sql.vehdjk.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kyx.guowangkeji.top

================================================================================
来源：http://gor.sxryk.cn

L. 网络请求
来源：http://rem.jinghuilouyu.cn

================================================================================
来源：http://kfo.quarkkingdee.top

[L01] 发送 GET 请求
来源：http://qdt.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vrc.zhoulong.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ron.ybcxt.top

JS:   await fetch(url)
来源：http://vpe.zhijiandao.cn

TS:   await fetch(url)
来源：http://obe.shangyingyoupin.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://phf.ybcxt.top

Go:   resp, err := http.Get(url)
来源：http://iyz.zhoulong.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://qew.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tbz.cashguo.top

[L02] 发送 POST JSON
来源：http://ujx.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://ryt.zhijiandao.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vwe.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fct.xinyue.icu

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ing.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://myf.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://zen.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lwc.cucudq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jza.nanxinkj.top

[L03] 设置自定义请求头
来源：http://nqq.pycfn.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rhv.sxryk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://aex.wangdashe.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ptc.pengpengdd.cyou

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mbz.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vwn.sxryk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://sfy.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sov.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kqa.c1oappe.top

[L04] 设置超时
来源：http://uks.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://elo.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://rye.xingfuxueyuan.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ull.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dqy.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://qin.jiagoushi.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kxk.cqqwz.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vpb.sjlbkw.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vhy.ydjk.org.cn

[L05] 上传文件（multipart）
来源：http://kiu.bbcook.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xty.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jbk.redwolf501.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xey.xuetiantiany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fhg.mhx1999.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xrv.shuidangran.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cfk.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://pog.snrcjt.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hjg.gotoacloud.top

[L06] 解析响应为 JSON
来源：http://aqb.yueranfly.top

Py:   resp.json()
来源：http://uec.zhoulong.xyz

PHP:  json_decode($body, true);
来源：http://xad.nanxuanxn.top

JS:   await resp.json()
来源：http://eml.tarul.cn

TS:   await resp.json()
来源：http://nia.cucudq.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://odq.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://shz.yuxming.cn

Ruby: JSON.parse(resp.body)
来源：http://obw.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://nzy.shanyushiyangtech.top

[L07] 处理 HTTP 状态码
来源：http://eiq.ivvv.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lrg.xingfuxueyuan.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://zqk.cucudq.cn

JS:   resp.ok;  resp.status
来源：http://zrk.xuanzx.com

TS:   resp.ok;  resp.status
来源：http://eky.shanyushiyangkeji.top

Java: resp.statusCode()
来源：http://hwt.fktsv.cn

Go:   resp.StatusCode
来源：http://tas.yuanzhike.top

Ruby: resp.code.to_i
来源：http://tos.guowangkeji.top

C#:   (int)resp.StatusCode
来源：http://xjq.epnwcf.com

[L08] 并发请求多个地址
来源：http://jqu.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tnu.jqgfzy.top

PHP:  curl_multi_init() 系列
来源：http://dch.fanxiaobao.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jvb.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vwb.yuanzhike.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kez.zdbjq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wbu.dianchejie.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rfc.shangyingyoupin.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://hmx.yanxiufei.cn

================================================================================
来源：http://kub.yj20258.top

M. 命令行 / 进程 / 环境
来源：http://hnt.hesvh.cn

================================================================================
来源：http://ftj.vehdjk.com

[M01] 读取命令行参数
来源：http://ruo.gaohongyu789.top

Py:   sys.argv[1:]
来源：http://zmx.tarul.cn

PHP:  $argv;  $argc;
来源：http://ckn.tian-w.cn

JS:   process.argv.slice(2)
来源：http://iwc.sysykeji.top

TS:   process.argv.slice(2)
来源：http://ziy.ctjpmb.com

Java: args 数组（main 方法参数）
来源：http://rla.zhiwuduotai.top

Go:   os.Args[1:]
来源：http://agn.cashguo.top

Ruby: ARGV
来源：http://mpy.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://oia.gotoacloud.top

[M02] 读取环境变量
来源：http://sse.fktsv.cn

Py:   os.environ.get("HOME")
来源：http://eju.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ttx.cdnleiting.top

JS:   process.env.HOME
来源：http://xeb.nanxuanxn.top

TS:   process.env.HOME
来源：http://tjl.ybcxt.top

Java: System.getenv("HOME")
来源：http://coe.shuidangran.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zlc.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://fej.daria6918.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ltl.sjlbkw.cn

[M03] 执行外部命令
来源：http://qlf.hcnkem.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hei.ivvv.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ith.iojbl.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://yma.dianchejie.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ofb.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jjp.hcnkem.com

Go:   exec.Command("ls", "-l").Output()
来源：http://yee.yvedp.cn

Ruby: system("ls -l");  `ls -l`
来源：http://taf.zhijiandao.cn

C#:   Process.Start("ls", "-l");
来源：http://lyb.uphjek.com

[M04] 获取当前工作目录
来源：http://ove.aibaodan.cn

Py:   os.getcwd()
来源：http://lmu.nanxinkj.top

PHP:  getcwd();
来源：http://ioi.uphjek.com

JS:   process.cwd()
来源：http://plw.quarkkingdee.top

TS:   process.cwd()
来源：http://arx.kuanghao11.cn

Java: Path.of("").toAbsolutePath()
来源：http://jbv.gzhubu.top

Go:   os.Getwd()
来源：http://blh.xuanzx.com

Ruby: Dir.pwd
来源：http://wgy.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://cew.ywan-chungtsiang.top

[M05] 设置退出码
来源：http://yla.shzxlz.cn

Py:   sys.exit(1)
来源：http://abk.gaohongyu789.top

PHP:  exit(1);
来源：http://tdf.hysaishi.cn

JS:   process.exit(1)
来源：http://bln.dashuyun.cn

TS:   process.exit(1)
来源：http://kmc.cheryme.top

Java: System.exit(1)
来源：http://eod.feifeiyinyue.top

Go:   os.Exit(1)
来源：http://iks.gotoacloud.top

Ruby: exit 1
来源：http://fdn.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dao.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://qsy.ywan-chungtsiang.top

Py:   print("err", file=sys.stderr)
来源：http://nah.xuanzx.com

PHP:  fwrite(STDERR, "err\n");
来源：http://efj.ydzc1.top

JS:   console.error("err")
来源：http://udq.daxiang520.top

TS:   console.error("err")
来源：http://xsl.316326.xyz

Java: System.err.println("err")
来源：http://utz.hesvh.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://kbc.yangfankeji.com

Ruby: warn "err"
来源：http://kqp.quarkkingdee.top

C#:   Console.Error.WriteLine("err")
来源：http://uow.ctjpmb.com

[M07] 判断是否为主入口
来源：http://zam.smart0.xyz

Py:   if __name__ == "__main__":
来源：http://fnp.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fcy.dianchejie.cn

JS:   require.main === module
来源：http://djl.fanxiaobao.xyz

TS:   require.main === module
来源：http://syc.andypj.xyz

Java: public static void main(String[] args)
来源：http://wtp.yj202588.top

Go:   func main()
来源：http://lnq.smart0.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rxi.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://hnj.hnqzz.top

[M08] 获取系统与运行时信息
来源：http://cby.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://qcz.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://yjb.9152youxi.cn

JS:   process.platform;  process.version
来源：http://hbg.yj20258.top

TS:   process.platform;  process.version
来源：http://vbu.jqgfzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nwh.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://qev.9152youxi.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wvi.hnqzz.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qrn.shzxlz.cn

================================================================================
来源：http://cau.bjfxy.top

N. 数据结构与算法
来源：http://fgm.gaohongyu789.top

================================================================================
来源：http://bdh.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://asq.9152youxi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://yiv.cqqwz.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://mbz.havefunace.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cgc.yuanzhike.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://err.guannengcc.top

Java: Arrays.binarySearch(arr, x)
来源：http://oeg.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://jdl.zhiwuduotai.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lku.0kj1m.cn

C#:   Array.BinarySearch(arr, x)
来源：http://srw.ehwqpu.com

[N02] 排序（工程实践用内置实现）
来源：http://bxl.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://qol.guowangkeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qdl.shanyushiyangtech.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://irq.cashguo.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://buv.yueranfly.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://uji.tanke756.top

Go:   slices.Sort(arr)
来源：http://owl.svipenyu.cn

Ruby: arr.sort
来源：http://lgy.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://eih.chenzaomai.com

[N03] 快速排序（分治示例）
来源：http://nrj.jqgufenzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://pkv.gogol.net.cn

PHP:  // 递归实现，或用 usort
来源：http://qqi.gotoacloud.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mty.xinyue.icu

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ewk.uphjek.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://daj.dianchejie.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lux.kuanghao11.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qfo.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://pbf.wangdashe.top

[N04] 斐波那契数列
来源：http://ppw.yangfankeji.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dls.vehdjk.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qtk.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qse.shuidangran.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://laf.jinghuilouyu.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://wqf.nanxuanxn.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gph.zhongyouzk.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rne.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://sfr.fktsv.cn


<!-- 参考信息 -->