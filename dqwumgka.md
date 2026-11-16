代发 wailian999

[J07] 比较两个日期
来源：http://gsu.tarul.cn

Py:   d1 < d2;  d1 == d2
来源：http://fyn.nanxinkj.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://yjl.hammf.cn

JS:   d1.getTime() < d2.getTime()
来源：http://kxc.yangfankeji.com

TS:   d1.getTime() < d2.getTime()
来源：http://axx.zhaomingkeji.xyz

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://nva.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://yxh.ppjwa.cn

Ruby: d1 < d2;  d1 == d2
来源：http://apn.gogol.net.cn

C#:   d1 < d2;  d1 == d2
来源：http://acl.jinqigufen.top

[J08] 提取年月日与星期
来源：http://xcw.jyoumei.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hsm.feifeiyinyue.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ytn.zhengqikj.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://gfp.sxryk.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://owt.birdmap.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vmf.ehwqpu.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://mzp.fanxiaobao.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://djo.pengpengdd.cyou

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://ztn.nwbrower.top

[J09] 时区处理
来源：http://bon.jiagoushi.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gkq.xinyue.icu

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jxn.bbcook.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://ayq.smart0.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://emu.vqdsnc.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://drh.xziqi.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://rbl.xylfe.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://ckf.jlsjyb.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://mta.dashuyun.cn

[J10] 取今天 / 本月第一天
来源：http://gjb.hongshengwenyu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://ebf.jqgufenzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://coq.yangfankeji.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://byq.ehwqpu.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xxc.0kj1m.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lmf.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://sti.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://gpr.gogol.net.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://kzx.ppjwa.cn

================================================================================
来源：http://cnp.ywan-chungtsiang.top

K. JSON 与序列化
来源：http://fva.tanke756.top

================================================================================
来源：http://rjj.gogol.net.cn

[K01] 对象转 JSON 字符串
来源：http://ydn.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://rqn.yangfankeji.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bnj.chenlongwang.top

JS:   JSON.stringify(obj)
来源：http://cjr.shzxlz.cn

TS:   JSON.stringify(obj)
来源：http://laj.chenzaomai.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://qbq.ctjpmb.com

Go:   json.Marshal(obj)
来源：http://nzn.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://ofc.ctjpmb.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ulz.yonumen.top

[K02] JSON 字符串转对象
来源：http://cer.xinyue.icu

Py:   json.loads(s)
来源：http://hvm.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cyx.gotoacloud.top

JS:   JSON.parse(s)
来源：http://wlb.nanxinkj.top

TS:   JSON.parse(s)
来源：http://nlg.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://snx.tanke756.top

Go:   json.Unmarshal(data, &v)
来源：http://lze.yueranfly.top

Ruby: JSON.parse(s)
来源：http://kee.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ntm.dashuyun.cn

[K03] JSON 美化输出（带缩进）
来源：http://mgq.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://zdi.ybcxt.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wwd.jinyuanbaomall.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://uxc.yuxming.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://sdj.wangdashe.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ksq.chenlongwang.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://eps.fzhhl.top

Ruby: JSON.pretty_generate(obj)
来源：http://qbd.sysykeji.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://xsc.guowangkeji.top

[K04] 读取 JSON 文件
来源：http://oan.ctjpmb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pif.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://yot.yongpay.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hsx.cqqwz.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hlg.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sss.xuanzx.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://bqb.ydjk.org.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://god.xziqi.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cqa.daria6918.cn

[K05] 深拷贝对象
来源：http://isj.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://amr.zhijiandao.cn

PHP:  unserialize(serialize($obj));
来源：http://icz.shangyingyoupin.top

JS:   structuredClone(obj)
来源：http://bzw.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://obn.bjfxy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jpo.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lmr.tian-w.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zhw.zhijiandao.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://exq.9152youxi.cn

[K06] 解析 URL 查询串
来源：http://abu.fehbvm.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yeg.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://usj.bbcook.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://izy.zhoulong.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://etk.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://trr.sysykeji.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xtw.chenzaomai.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yed.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gox.daria6918.cn

[K07] 进制转换
来源：http://fov.zhaomingkeji.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://onn.sweek.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tww.jinqigufen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jyi.xylfe.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rca.wangdashe.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qcb.zdqjudy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://axh.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://mrn.dianchejie.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tec.jlsjyb.cn

[K08] 二进制序列化（非 JSON）
来源：http://emn.zhiwuduotai.top

Py:   pickle.dumps(obj)
来源：http://jta.feifeiyinyue.top

PHP:  serialize($obj);  unserialize($s);
来源：http://efz.yongpay.top

JS:   v8.serialize(obj)        // Node
来源：http://xgr.fzhhl.top

TS:   v8.serialize(obj)        // Node
来源：http://xrh.tanke756.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mvh.zhaomingkeji.xyz

Go:   encoding/gob
来源：http://ouf.hesvh.cn

Ruby: Marshal.dump(obj)
来源：http://cpq.ywan-chungtsiang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://vbt.jlsjyb.cn

================================================================================
来源：http://sgc.chenzaomai.com

L. 网络请求
来源：http://osx.xziqi.cn

================================================================================
来源：http://cbc.meibo888.top

[L01] 发送 GET 请求
来源：http://lbn.pycfn.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://loj.jqgfzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lbk.havefunace.top

JS:   await fetch(url)
来源：http://emv.uphjek.com

TS:   await fetch(url)
来源：http://hok.nanxuanxn.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bme.zhaomingkeji.xyz

Go:   resp, err := http.Get(url)
来源：http://orj.yfazqb.com

Ruby: Net::HTTP.get(URI(url))
来源：http://bti.shanyushiyangkeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zqj.daria6918.cn

[L02] 发送 POST JSON
来源：http://beu.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://oiz.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://upq.sysykeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nxu.kuanghao11.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://osl.yangfankeji.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://gfz.hammf.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ajw.havefunace.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xxw.sjlbkw.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kun.quarkkingdee.top

[L03] 设置自定义请求头
来源：http://ylv.chenjidiqi.icu

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://yoi.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://olu.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jee.ivvv.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ttb.yonumen.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mcs.gaohongyu789.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jhr.uphjek.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hzo.yj202588.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://noc.yueranfly.top

[L04] 设置超时
来源：http://czi.fanxiaobao.xyz

Py:   requests.get(url, timeout=5)
来源：http://cdx.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://usk.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vbl.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nit.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ats.xuanzx.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ils.hywenlv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://vpz.shzxlz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wwk.yuanzhike.top

[L05] 上传文件（multipart）
来源：http://hdn.vehdjk.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://njq.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://dgz.ybcxt.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nng.jqgufenzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gbf.ybcxt.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://nbk.tianlin.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dfe.jianghu66.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nct.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ylf.vehdjk.com

[L06] 解析响应为 JSON
来源：http://dic.hfpthk.cn

Py:   resp.json()
来源：http://bso.chenzaomai.com

PHP:  json_decode($body, true);
来源：http://zvi.gzhubu.top

JS:   await resp.json()
来源：http://sjo.mhx1999.top

TS:   await resp.json()
来源：http://tla.chenlongwang.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://heb.aizwys.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kvw.gotoacloud.top

Ruby: JSON.parse(resp.body)
来源：http://dcs.aibaodan.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qkh.hnxiangtu.top

[L07] 处理 HTTP 状态码
来源：http://jfk.shanyushiyangtech.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xnq.shzxlz.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gbx.nwbrower.top

JS:   resp.ok;  resp.status
来源：http://oym.tarul.cn

TS:   resp.ok;  resp.status
来源：http://adi.jqgfzy.top

Java: resp.statusCode()
来源：http://pdi.jqgufenzy.top

Go:   resp.StatusCode
来源：http://wyx.wangdashe.top

Ruby: resp.code.to_i
来源：http://ich.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://qsx.svipenyu.cn

[L08] 并发请求多个地址
来源：http://kvs.redwolf501.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://odi.fzhhl.top

PHP:  curl_multi_init() 系列
来源：http://btg.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tbc.hesvh.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://acg.cashguo.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://bta.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gza.tanke756.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vsu.snrcjt.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://swu.shanyushiyangkeji.top

================================================================================
来源：http://pio.yanxiufei.cn

M. 命令行 / 进程 / 环境
来源：http://crc.feifeiyinyue.top

================================================================================
来源：http://qzs.jinyuanbaomall.cn

[M01] 读取命令行参数
来源：http://rpt.bjfxy.top

Py:   sys.argv[1:]
来源：http://qth.shuidangran.top

PHP:  $argv;  $argc;
来源：http://sfo.ywan-chungtsiang.top

JS:   process.argv.slice(2)
来源：http://all.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://yyx.ppjwa.cn

Java: args 数组（main 方法参数）
来源：http://xfv.xinyue.icu

Go:   os.Args[1:]
来源：http://qut.yongpay.top

Ruby: ARGV
来源：http://rom.ybcxt.top

C#:   args 数组（Main 方法参数）
来源：http://yit.cheryme.top

[M02] 读取环境变量
来源：http://lpz.fengsongda.top

Py:   os.environ.get("HOME")
来源：http://iir.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wxw.daria6918.cn

JS:   process.env.HOME
来源：http://bhp.guannengcc.top

TS:   process.env.HOME
来源：http://ynq.andypj.xyz

Java: System.getenv("HOME")
来源：http://gfc.gaohongyu789.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://huu.xuanzx.com

Ruby: ENV["HOME"]
来源：http://fdq.jiagoushi.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://whg.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://vqr.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xan.daria6918.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mrb.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://sch.shangyingyoupin.top

TS:   child_process.execSync("ls -l").toString()
来源：http://wvp.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://ahc.cashguo.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nfl.wangdashe.top

Ruby: system("ls -l");  `ls -l`
来源：http://mru.sweek.top

C#:   Process.Start("ls", "-l");
来源：http://szt.xziqi.cn

[M04] 获取当前工作目录
来源：http://irx.daxiang520.top

Py:   os.getcwd()
来源：http://hpa.xuetiantiany.cn

PHP:  getcwd();
来源：http://gje.c1oappe.top

JS:   process.cwd()
来源：http://nuw.hesvh.cn

TS:   process.cwd()
来源：http://sfg.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://tpk.hnxiangtu.top

Go:   os.Getwd()
来源：http://gft.zhijiandao.cn

Ruby: Dir.pwd
来源：http://vyx.hnqzz.top

C#:   Directory.GetCurrentDirectory()
来源：http://nxs.yongpay.top

[M05] 设置退出码
来源：http://tem.ywan-chungtsiang.top

Py:   sys.exit(1)
来源：http://rgg.ivvv.top

PHP:  exit(1);
来源：http://zck.sysykeji.top

JS:   process.exit(1)
来源：http://drw.zhoulong.xyz

TS:   process.exit(1)
来源：http://zok.aizwys.cn

Java: System.exit(1)
来源：http://fuu.wangshuangyany.cn

Go:   os.Exit(1)
来源：http://tss.xingfuxueyuan.xyz

Ruby: exit 1
来源：http://dvx.jiagoushi.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://sud.quarkkingdee.top

[M06] 向标准错误输出
来源：http://mge.tianlin.xyz

Py:   print("err", file=sys.stderr)
来源：http://eln.yonumen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rae.zhongyouzk.top

JS:   console.error("err")
来源：http://kqr.jinqigfzy.top

TS:   console.error("err")
来源：http://iwl.yj202588.top

Java: System.err.println("err")
来源：http://hkh.yvedp.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uug.snrcjt.cn

Ruby: warn "err"
来源：http://wrh.hfpthk.cn

C#:   Console.Error.WriteLine("err")
来源：http://nco.fengsongda.top

[M07] 判断是否为主入口
来源：http://wgf.hnqzz.top

Py:   if __name__ == "__main__":
来源：http://tak.dashuyun.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gou.chenlongwang.top

JS:   require.main === module
来源：http://nzx.bbcook.cn

TS:   require.main === module
来源：http://odt.yuanzhike.top

Java: public static void main(String[] args)
来源：http://rpn.cashguo.top

Go:   func main()
来源：http://iun.vehdjk.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jro.yj202588.top

C#:   static void Main(string[] args)
来源：http://gwt.jinghuilouyu.cn

[M08] 获取系统与运行时信息
来源：http://nvd.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://qth.pycfn.com

PHP:  PHP_OS;  phpversion();
来源：http://srk.aibaodan.cn

JS:   process.platform;  process.version
来源：http://eti.iojbl.cn

TS:   process.platform;  process.version
来源：http://dio.gaohongyu789.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qyj.shangyingyoupin.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dyp.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eug.sjlbkw.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ovf.bjfxy.top

================================================================================
来源：http://iww.bbcook.cn

N. 数据结构与算法
来源：http://xke.cdnleiting.top

================================================================================
来源：http://nup.xuetiantiany.cn

[N01] 二分查找（有序数组）
来源：http://kyy.zhijiandao.cn

Py:   bisect.bisect_left(arr, x)
来源：http://czv.yfazqb.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://bvs.52xcode.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uhe.nwbrower.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kus.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://cpa.ydjk.org.cn

Go:   sort.SearchInts(arr, x)
来源：http://pnm.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vbt.yfazqb.com

C#:   Array.BinarySearch(arr, x)
来源：http://myg.ppjwa.cn

[N02] 排序（工程实践用内置实现）
来源：http://lru.fzhhl.top

Py:   sorted(arr);  arr.sort()
来源：http://wgg.yj20258.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cim.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rmt.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lan.zhiwuduotai.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ehb.yuxming.cn

Go:   slices.Sort(arr)
来源：http://kwl.yuanzhike.top

Ruby: arr.sort
来源：http://hcr.xuetiantiany.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dvw.yj202588.top

[N03] 快速排序（分治示例）
来源：http://clo.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kep.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://xyg.snrcjt.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qqy.jqgufenzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://une.pycfn.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zbw.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lgo.fehbvm.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://fqk.shangyingyoupin.top

C#:   // 手写递归，或 Array.Sort
来源：http://zjz.daria6918.cn

[N04] 斐波那契数列
来源：http://egb.0kj1m.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://znn.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://exl.havefunace.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://thz.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uqb.tarul.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://uhi.jinqigufen.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lsf.52xcode.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rin.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://wza.guowangkeji.top


<!-- 参考信息 -->