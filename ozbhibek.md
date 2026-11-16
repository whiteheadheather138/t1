代发 wailian999

Java: Duration.between(start, end).toSeconds()
来源：http://azw.zhixingplan.top

Go:   end.Sub(start).Hours()
来源：http://kek.daria6918.cn

Ruby: end - start                 # 返回秒数
来源：http://igf.yvedp.cn

C#:   (end - start).TotalSeconds
来源：http://ohc.jqgfzy.top

[J07] 比较两个日期
来源：http://keg.hongshengwenyu.top

Py:   d1 < d2;  d1 == d2
来源：http://xow.daria6918.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://sva.shangyingyoupin.top

JS:   d1.getTime() < d2.getTime()
来源：http://exb.zhijiandao.cn

TS:   d1.getTime() < d2.getTime()
来源：http://sxh.hfpthk.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://xnz.sxryk.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://xve.yangfankeji.com

Ruby: d1 < d2;  d1 == d2
来源：http://szb.cqqwz.cn

C#:   d1 < d2;  d1 == d2
来源：http://bdj.hnqzz.top

[J08] 提取年月日与星期
来源：http://zwh.xylfe.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://opm.chenzaomai.com

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://lwa.zdqjudy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nvw.shzxlz.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://scw.tanke756.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://sia.yj20258.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qed.epnwcf.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://hsc.shangyingyoupin.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://dwi.yvedp.cn

[J09] 时区处理
来源：http://oiq.nanxuanxn.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://qjp.zdqjudy.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://rfw.ydjk.org.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://hqn.fanxiaobao.xyz

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fba.bjfxy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://qxz.jinghuilouyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://oop.yanxiufei.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://rql.fengsongda.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://fym.hongshengwenyu.top

[J10] 取今天 / 本月第一天
来源：http://yyt.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://blz.hammf.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fpf.zycfv.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://oib.aibaodan.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ddl.hywenlv.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xhs.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bzu.fzhhl.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ctj.nanxuanxn.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xzl.jinqigfzy.top

================================================================================
来源：http://ooc.ctjpmb.com

K. JSON 与序列化
来源：http://rxx.mhx1999.top

================================================================================
来源：http://cjz.fktsv.cn

[K01] 对象转 JSON 字符串
来源：http://ozi.sjlbkw.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lmd.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ucl.gzhubu.top

JS:   JSON.stringify(obj)
来源：http://hha.bjfxy.top

TS:   JSON.stringify(obj)
来源：http://dmj.gzhubu.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xpf.hongshengwenyu.top

Go:   json.Marshal(obj)
来源：http://qdf.hammf.cn

Ruby: obj.to_json                                     // require "json"
来源：http://usa.yj20258888.top

C#:   JsonSerializer.Serialize(obj)
来源：http://mzs.ybcxt.top

[K02] JSON 字符串转对象
来源：http://uik.guannengcc.top

Py:   json.loads(s)
来源：http://cfq.sxryk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xfa.ppjwa.cn

JS:   JSON.parse(s)
来源：http://zex.hcnkem.com

TS:   JSON.parse(s)
来源：http://gum.xziqi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ybe.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://xvd.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://lbp.cheryme.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cab.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://ykr.cucudq.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kry.tian-w.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pwn.hcnkem.com

JS:   JSON.stringify(obj, null, 2)
来源：http://auo.yangfankeji.com

TS:   JSON.stringify(obj, null, 2)
来源：http://hok.tarul.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zpc.ydzc1.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qdj.ywan-chungtsiang.top

Ruby: JSON.pretty_generate(obj)
来源：http://zpg.yonumen.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lks.shanyushiyangkeji.top

[K04] 读取 JSON 文件
来源：http://awa.ehwqpu.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vbv.ehwqpu.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://llg.dianchejie.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dsu.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://owe.svipenyu.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hfr.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zxv.gaohongyu789.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fap.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://myx.andypj.xyz

[K05] 深拷贝对象
来源：http://ruu.xinyue.icu

Py:   copy.deepcopy(obj)
来源：http://muf.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://olr.pengpengdd.cyou

JS:   structuredClone(obj)
来源：http://joe.quarkkingdee.top

TS:   structuredClone(obj)
来源：http://npx.52xcode.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://iue.yangfankeji.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://vtj.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://spc.cqqwz.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://zxo.daria6918.cn

[K06] 解析 URL 查询串
来源：http://ody.aibaodan.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kcl.smart0.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ugq.zhiwuduotai.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yom.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nqe.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://axu.yangfankeji.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://dzb.daxiang520.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gew.cqqwz.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pea.redwolf501.top

[K07] 进制转换
来源：http://emm.dianchejie.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nmx.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vhy.zhoulong.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vkg.haohaochexian.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qxu.iojbl.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fdt.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hmt.tianlin.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yck.fehbvm.com

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qkp.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://agq.gotoacloud.top

Py:   pickle.dumps(obj)
来源：http://ncu.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://adr.kuanghao11.cn

JS:   v8.serialize(obj)        // Node
来源：http://fjl.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://kib.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yyq.hysaishi.cn

Go:   encoding/gob
来源：http://zmy.xinyue.icu

Ruby: Marshal.dump(obj)
来源：http://zvu.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wpw.shanyushiyangkeji.top

================================================================================
来源：http://mvo.daria6918.cn

L. 网络请求
来源：http://img.ehwqpu.com

================================================================================
来源：http://axa.ybcxt.top

[L01] 发送 GET 请求
来源：http://slj.hnqzz.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gfk.tarul.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qim.zdqjudy.top

JS:   await fetch(url)
来源：http://czf.ehwqpu.com

TS:   await fetch(url)
来源：http://qrm.yongpay.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lev.iojbl.cn

Go:   resp, err := http.Get(url)
来源：http://pjf.jlsjyb.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zdw.yanxiufei.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hnf.aizwys.cn

[L02] 发送 POST JSON
来源：http://lrm.jyoumei.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fgc.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tbz.zhengqikj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gve.hywenlv.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qvz.xziqi.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://asb.316326.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kuy.xziqi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dbz.zdbjq.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wee.yj202588.top

[L03] 设置自定义请求头
来源：http://lza.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jst.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fbw.cqqwz.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mlz.quarkkingdee.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ymk.yvedp.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gaj.xingfuxueyuan.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cor.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://afz.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jxe.xinyue.icu

[L04] 设置超时
来源：http://bft.ivvv.top

Py:   requests.get(url, timeout=5)
来源：http://ses.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://idf.yangfankeji.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fch.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jue.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://njh.aizwys.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ogi.jinyuanbaomall.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fpf.cdnleiting.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rpt.aibaodan.cn

[L05] 上传文件（multipart）
来源：http://nxr.xuetiantiany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jog.gogol.net.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://yzt.bbcook.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fad.nanxuanxn.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://lmr.xylfe.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wbm.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lpt.tarul.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qyo.zhiwuduotai.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ooy.wangshuangyany.cn

[L06] 解析响应为 JSON
来源：http://ujj.wangdashe.top

Py:   resp.json()
来源：http://uyy.jinqigufen.top

PHP:  json_decode($body, true);
来源：http://fxx.fehbvm.com

JS:   await resp.json()
来源：http://jck.chenzaomai.com

TS:   await resp.json()
来源：http://gdu.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kab.zhaomingkeji.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ijz.yj20258.top

Ruby: JSON.parse(resp.body)
来源：http://ojn.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://fwk.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://tkk.jyoumei.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kar.hcnkem.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://clc.bbcook.cn

JS:   resp.ok;  resp.status
来源：http://hyu.yanxiufei.cn

TS:   resp.ok;  resp.status
来源：http://pcp.vqdsnc.cn

Java: resp.statusCode()
来源：http://qqb.aibaodan.cn

Go:   resp.StatusCode
来源：http://ddv.bbcook.cn

Ruby: resp.code.to_i
来源：http://akp.yonumen.top

C#:   (int)resp.StatusCode
来源：http://pnv.nanxuanxn.top

[L08] 并发请求多个地址
来源：http://lsp.wangdashe.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dta.jinyuanbaomall.cn

PHP:  curl_multi_init() 系列
来源：http://jwq.jyoumei.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://iuh.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nyu.pengpengdd.cyou

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rpg.jinqigufen.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://aua.zhiwuduotai.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xcw.sufxvd.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gym.jiagoushi.top

================================================================================
来源：http://wqq.haohaochexian.top

M. 命令行 / 进程 / 环境
来源：http://tzb.bbcook.cn

================================================================================
来源：http://dtz.shangyingyoupin.top

[M01] 读取命令行参数
来源：http://lxc.bbcook.cn

Py:   sys.argv[1:]
来源：http://dif.zhongyouzk.top

PHP:  $argv;  $argc;
来源：http://gkn.cheryme.top

JS:   process.argv.slice(2)
来源：http://usw.gaohongyu789.top

TS:   process.argv.slice(2)
来源：http://rmj.tanke756.top

Java: args 数组（main 方法参数）
来源：http://gcf.ppjwa.cn

Go:   os.Args[1:]
来源：http://wfr.ydzc1.top

Ruby: ARGV
来源：http://cxd.hysaishi.cn

C#:   args 数组（Main 方法参数）
来源：http://zvl.jinqigfzy.top

[M02] 读取环境变量
来源：http://oqw.mhx1999.top

Py:   os.environ.get("HOME")
来源：http://rkv.tarul.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gym.bbcook.cn

JS:   process.env.HOME
来源：http://pgy.hcnkem.com

TS:   process.env.HOME
来源：http://jsf.yvedp.cn

Java: System.getenv("HOME")
来源：http://utn.cheryme.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://owv.chenjidiqi.icu

Ruby: ENV["HOME"]
来源：http://lql.uphjek.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bqp.9152youxi.cn

[M03] 执行外部命令
来源：http://pdm.sweek.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xob.chenzaomai.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kux.cdnleiting.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ghe.hesvh.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ipo.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kjg.ehwqpu.com

Go:   exec.Command("ls", "-l").Output()
来源：http://mgc.zycfv.cn

Ruby: system("ls -l");  `ls -l`
来源：http://wqz.shzxlz.cn

C#:   Process.Start("ls", "-l");
来源：http://sri.jinyuanbaomall.cn

[M04] 获取当前工作目录
来源：http://qpo.yangfankeji.com

Py:   os.getcwd()
来源：http://wiv.hysaishi.cn

PHP:  getcwd();
来源：http://gmr.hnxiangtu.top

JS:   process.cwd()
来源：http://pvv.jinqigufen.top

TS:   process.cwd()
来源：http://rge.yj202588.top

Java: Path.of("").toAbsolutePath()
来源：http://wlx.sxryk.cn

Go:   os.Getwd()
来源：http://vpe.xuanzx.com

Ruby: Dir.pwd
来源：http://ckt.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://yci.yj20258.top

[M05] 设置退出码
来源：http://opu.meibo888.top

Py:   sys.exit(1)
来源：http://ezg.zhiwuduotai.top

PHP:  exit(1);
来源：http://qqx.yj20258.top

JS:   process.exit(1)
来源：http://jox.tianlin.xyz

TS:   process.exit(1)
来源：http://bld.yj20258.top

Java: System.exit(1)
来源：http://edp.zhiwuduotai.top

Go:   os.Exit(1)
来源：http://duo.zycfv.cn

Ruby: exit 1
来源：http://lxx.daxiang520.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://psj.jinyuanbaomall.cn

[M06] 向标准错误输出
来源：http://apz.sxryk.cn

Py:   print("err", file=sys.stderr)
来源：http://kha.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://otr.yuxming.cn

JS:   console.error("err")
来源：http://pos.yongpay.top

TS:   console.error("err")
来源：http://adq.chenlongwang.top

Java: System.err.println("err")
来源：http://ale.fehbvm.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://mmd.birdmap.top

Ruby: warn "err"
来源：http://sbm.pengpengdd.cyou

C#:   Console.Error.WriteLine("err")
来源：http://vcl.yfazqb.com

[M07] 判断是否为主入口
来源：http://ezx.316326.xyz

Py:   if __name__ == "__main__":
来源：http://pqc.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://xuk.svipenyu.cn

JS:   require.main === module
来源：http://ddv.feifeiyinyue.top

TS:   require.main === module
来源：http://jng.snrcjt.cn

Java: public static void main(String[] args)
来源：http://oqh.zhijiandao.cn

Go:   func main()
来源：http://hin.iojbl.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hgu.ctjpmb.com

C#:   static void Main(string[] args)
来源：http://tmp.zhaomingkeji.xyz

[M08] 获取系统与运行时信息
来源：http://hsr.shuidangran.top

Py:   platform.system();  platform.python_version()
来源：http://spr.aizwys.cn

PHP:  PHP_OS;  phpversion();
来源：http://hzy.pengpengdd.cyou

JS:   process.platform;  process.version
来源：http://adt.xinyue.icu

TS:   process.platform;  process.version
来源：http://psd.fanxiaobao.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://pxj.iojbl.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://yzz.nanxuanxn.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zgb.tianlin.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://heg.yfazqb.com

================================================================================
来源：http://dey.yfazqb.com

N. 数据结构与算法
来源：http://fdg.chenlongwang.top

================================================================================
来源：http://bsi.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://yow.iojbl.cn

Py:   bisect.bisect_left(arr, x)
来源：http://gtu.xinyue.icu

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dos.hfpthk.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ekm.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jgq.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ntw.zhijiandao.cn

Go:   sort.SearchInts(arr, x)
来源：http://ukf.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://gbs.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://wcm.chenlongwang.top

[N02] 排序（工程实践用内置实现）
来源：http://hyh.wangdashe.top

Py:   sorted(arr);  arr.sort()
来源：http://kub.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gmf.316326.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://aqv.havefunace.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://trt.havefunace.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://stt.zhengqikj.top

Go:   slices.Sort(arr)
来源：http://klu.haohaochexian.top

Ruby: arr.sort
来源：http://nfr.wangdashe.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qrl.havefunace.top

[N03] 快速排序（分治示例）
来源：http://sbq.yongpay.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sxc.sufxvd.cn

PHP:  // 递归实现，或用 usort
来源：http://iul.bbcook.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uqs.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://dkw.bjfxy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://sno.shzxlz.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ran.iojbl.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wbz.fktsv.cn

C#:   // 手写递归，或 Array.Sort
来源：http://xvg.tianlin.xyz

[N04] 斐波那契数列
来源：http://uph.sxryk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ncz.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gki.xziqi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sds.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qou.shangyingyoupin.top


<!-- 参考信息 -->