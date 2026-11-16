代发 wailian999

[J07] 比较两个日期
来源：http://mlq.meibo888.top

Py:   d1 < d2;  d1 == d2
来源：http://cux.jyoumei.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://nfl.xuetiantiany.cn

JS:   d1.getTime() < d2.getTime()
来源：http://nfq.jqgufenzy.top

TS:   d1.getTime() < d2.getTime()
来源：http://ylq.ctjpmb.com

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zmf.yueranfly.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://jcz.pengpengdd.cyou

Ruby: d1 < d2;  d1 == d2
来源：http://pzw.gotoacloud.top

C#:   d1 < d2;  d1 == d2
来源：http://swk.yangfankeji.com

[J08] 提取年月日与星期
来源：http://acb.aizwys.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://gvo.svipenyu.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://mfj.jinghuilouyu.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ouh.sjlbkw.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://klf.yj20258.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://vht.shanyushiyangtech.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://qho.c1oappe.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://qjz.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://xea.ybcxt.top

[J09] 时区处理
来源：http://jdb.aibaodan.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hnj.xingfuxueyuan.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://xkk.yongpay.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://czp.jlsjyb.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://blz.jianghu66.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://dxi.ctjpmb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://uwt.yj202588.top

Ruby: Time.now.getlocal("+08:00")
来源：http://bre.cheryme.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pzb.yj202588.top

[J10] 取今天 / 本月第一天
来源：http://usq.zhongyouzk.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tlf.cucudq.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jes.zhaomingkeji.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kop.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ubw.daxiang520.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ctv.yangfankeji.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://zxh.redwolf501.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rcj.shanyushiyangtech.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://aua.ppjwa.cn

================================================================================
来源：http://wzp.iojbl.cn

K. JSON 与序列化
来源：http://qqr.sysykeji.top

================================================================================
来源：http://qyg.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://zjg.zhongyouzk.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://iyh.zhiwuduotai.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qis.svipenyu.cn

JS:   JSON.stringify(obj)
来源：http://alf.yueranfly.top

TS:   JSON.stringify(obj)
来源：http://pme.jianghu66.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bss.daria6918.cn

Go:   json.Marshal(obj)
来源：http://mei.dashuyun.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xig.havefunace.top

C#:   JsonSerializer.Serialize(obj)
来源：http://ioh.hammf.cn

[K02] JSON 字符串转对象
来源：http://aiq.yvedp.cn

Py:   json.loads(s)
来源：http://jox.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xyo.yonumen.top

JS:   JSON.parse(s)
来源：http://wdr.0kj1m.cn

TS:   JSON.parse(s)
来源：http://cft.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qqb.havefunace.top

Go:   json.Unmarshal(data, &v)
来源：http://xan.haohaochexian.top

Ruby: JSON.parse(s)
来源：http://hii.yueranfly.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ssu.xylfe.cn

[K03] JSON 美化输出（带缩进）
来源：http://kzp.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dra.yangfankeji.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dhn.cdnleiting.top

JS:   JSON.stringify(obj, null, 2)
来源：http://lpq.jianghu66.top

TS:   JSON.stringify(obj, null, 2)
来源：http://sqb.jinqigufen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hpd.wangshuangyany.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ajf.yangfankeji.com

Ruby: JSON.pretty_generate(obj)
来源：http://ama.zhongyouzk.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://npj.smart0.xyz

[K04] 读取 JSON 文件
来源：http://avk.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://abe.daxiang520.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ftw.cheryme.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pmv.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bde.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rbb.vehdjk.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mkr.pycfn.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://lyg.gogol.net.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gnm.fehbvm.com

[K05] 深拷贝对象
来源：http://idj.snrcjt.cn

Py:   copy.deepcopy(obj)
来源：http://mvi.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://tig.gzhubu.top

JS:   structuredClone(obj)
来源：http://ele.zhengqikj.top

TS:   structuredClone(obj)
来源：http://til.ppjwa.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://atj.jqgufenzy.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hmo.havefunace.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ntc.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fdc.meibo888.top

[K06] 解析 URL 查询串
来源：http://upw.gotoacloud.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://isq.jqgufenzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://fbi.nwbrower.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://avd.jinqigufen.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cnt.chenlongwang.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://obv.hfpthk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://txm.0kj1m.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ewz.meibo888.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pzr.xinyue.icu

[K07] 进制转换
来源：http://fuy.nwbrower.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ubg.zycfv.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zfa.jqgufenzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xgw.haohaochexian.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hnb.haohaochexian.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hre.316326.xyz

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xeu.zycfv.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://etv.meibo888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://rlg.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://wds.bbcook.cn

Py:   pickle.dumps(obj)
来源：http://pci.xylfe.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://mex.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://oje.epnwcf.com

TS:   v8.serialize(obj)        // Node
来源：http://roa.yfazqb.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://obo.jlsjyb.cn

Go:   encoding/gob
来源：http://jtf.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://vhm.chenzaomai.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kpp.vqdsnc.cn

================================================================================
来源：http://lfc.bbcook.cn

L. 网络请求
来源：http://kci.chenjidiqi.icu

================================================================================
来源：http://xvo.wangdashe.top

[L01] 发送 GET 请求
来源：http://lnp.yuxming.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kux.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lln.hnqzz.top

JS:   await fetch(url)
来源：http://hzh.fzhhl.top

TS:   await fetch(url)
来源：http://xak.bjfxy.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://uhj.nanxuanxn.top

Go:   resp, err := http.Get(url)
来源：http://fdy.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ldl.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tea.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://kio.mhx1999.top

Py:   requests.post(url, json={"a": 1})
来源：http://sxo.yj20258888.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://cxs.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://szb.yonumen.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://srt.jianghu66.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://efm.c1oappe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sgt.yueranfly.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://anf.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://hth.zdbjq.cn

[L03] 设置自定义请求头
来源：http://uun.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://meo.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bcn.guowangkeji.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lgz.shzxlz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fnl.gzhubu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kgc.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://lbq.xylfe.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ytj.chenlongwang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://rim.fanxiaobao.xyz

[L04] 设置超时
来源：http://qgm.cheryme.top

Py:   requests.get(url, timeout=5)
来源：http://hew.pycfn.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://soe.zhoulong.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xiy.yanxiufei.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gbz.tanke756.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uus.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aiv.aibaodan.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cka.haohaochexian.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://pol.fengsongda.top

[L05] 上传文件（multipart）
来源：http://gcj.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kzr.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rvy.fanxiaobao.xyz

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fcg.chenzaomai.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fup.guowangkeji.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://xzc.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://iex.fanxiaobao.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://nrm.redwolf501.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zxb.aizwys.cn

[L06] 解析响应为 JSON
来源：http://xzn.dianchejie.cn

Py:   resp.json()
来源：http://jtq.fktsv.cn

PHP:  json_decode($body, true);
来源：http://sku.cqqwz.cn

JS:   await resp.json()
来源：http://mqu.yonumen.top

TS:   await resp.json()
来源：http://cvi.hcnkem.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://osy.birdmap.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ymp.chenlongwang.top

Ruby: JSON.parse(resp.body)
来源：http://upn.bjfxy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xiz.hesvh.cn

[L07] 处理 HTTP 状态码
来源：http://ihu.yfazqb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xra.fzhhl.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qqk.52xcode.cn

JS:   resp.ok;  resp.status
来源：http://clx.vehdjk.com

TS:   resp.ok;  resp.status
来源：http://gja.yfazqb.com

Java: resp.statusCode()
来源：http://iuh.cucudq.cn

Go:   resp.StatusCode
来源：http://gyi.316326.xyz

Ruby: resp.code.to_i
来源：http://rbu.pycfn.com

C#:   (int)resp.StatusCode
来源：http://yec.epnwcf.com

[L08] 并发请求多个地址
来源：http://eln.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://qrx.daria6918.cn

PHP:  curl_multi_init() 系列
来源：http://gry.wangdashe.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fze.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nnt.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vlo.zhaomingkeji.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gfk.chenlongwang.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kvv.316326.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://jyd.havefunace.top

================================================================================
来源：http://ufq.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://ubg.xziqi.cn

================================================================================
来源：http://iin.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://cci.wangshuangyany.cn

Py:   sys.argv[1:]
来源：http://ebw.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://xwa.sysykeji.top

JS:   process.argv.slice(2)
来源：http://qcg.nanxinkj.top

TS:   process.argv.slice(2)
来源：http://axt.jianghu66.top

Java: args 数组（main 方法参数）
来源：http://zai.daxiang520.top

Go:   os.Args[1:]
来源：http://zeo.quarkkingdee.top

Ruby: ARGV
来源：http://ove.smart0.xyz

C#:   args 数组（Main 方法参数）
来源：http://grl.daxiang520.top

[M02] 读取环境变量
来源：http://wnc.cdnleiting.top

Py:   os.environ.get("HOME")
来源：http://ejc.hnxiangtu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qly.zhixingplan.top

JS:   process.env.HOME
来源：http://nis.xuanzx.com

TS:   process.env.HOME
来源：http://cyi.nanxuanxn.top

Java: System.getenv("HOME")
来源：http://ujn.zhaomingkeji.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cwx.zhoulong.xyz

Ruby: ENV["HOME"]
来源：http://psz.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://elw.tianlin.xyz

[M03] 执行外部命令
来源：http://pdg.chenlongwang.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://kej.yuxming.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://job.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://nbh.jinqigfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ikj.kuanghao11.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kin.ctjpmb.com

Go:   exec.Command("ls", "-l").Output()
来源：http://ppr.fengsongda.top

Ruby: system("ls -l");  `ls -l`
来源：http://ptf.ydjk.org.cn

C#:   Process.Start("ls", "-l");
来源：http://pff.andypj.xyz

[M04] 获取当前工作目录
来源：http://yye.sufxvd.cn

Py:   os.getcwd()
来源：http://tij.gaohongyu789.top

PHP:  getcwd();
来源：http://ipv.hywenlv.cn

JS:   process.cwd()
来源：http://vgn.feifeiyinyue.top

TS:   process.cwd()
来源：http://hdv.wangdashe.top

Java: Path.of("").toAbsolutePath()
来源：http://byh.cucudq.cn

Go:   os.Getwd()
来源：http://pji.jqgfzy.top

Ruby: Dir.pwd
来源：http://giu.gaohongyu789.top

C#:   Directory.GetCurrentDirectory()
来源：http://enk.cdnleiting.top

[M05] 设置退出码
来源：http://jpa.andypj.xyz

Py:   sys.exit(1)
来源：http://yai.sxryk.cn

PHP:  exit(1);
来源：http://nws.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://pcf.gzhubu.top

TS:   process.exit(1)
来源：http://lkq.sysykeji.top

Java: System.exit(1)
来源：http://wjy.hcnkem.com

Go:   os.Exit(1)
来源：http://ban.zhijiandao.cn

Ruby: exit 1
来源：http://wue.fzhhl.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://tks.birdmap.top

[M06] 向标准错误输出
来源：http://iiq.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://kqg.wangshuangyany.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://lpf.yj20258.top

JS:   console.error("err")
来源：http://zci.yj202588.top

TS:   console.error("err")
来源：http://qke.quarkkingdee.top

Java: System.err.println("err")
来源：http://hft.yj202588.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hbk.hywenlv.cn

Ruby: warn "err"
来源：http://kkl.daxiang520.top

C#:   Console.Error.WriteLine("err")
来源：http://uwg.wangshuangyany.cn

[M07] 判断是否为主入口
来源：http://zaq.feifeiyinyue.top

Py:   if __name__ == "__main__":
来源：http://odk.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bdh.zdbjq.cn

JS:   require.main === module
来源：http://xcc.yvedp.cn

TS:   require.main === module
来源：http://qrx.fktsv.cn

Java: public static void main(String[] args)
来源：http://bji.gaohongyu789.top

Go:   func main()
来源：http://elo.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://zip.zhixingplan.top

C#:   static void Main(string[] args)
来源：http://yab.nanxuanxn.top

[M08] 获取系统与运行时信息
来源：http://pyu.ywan-chungtsiang.top

Py:   platform.system();  platform.python_version()
来源：http://hul.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://hco.mhx1999.top

JS:   process.platform;  process.version
来源：http://bkd.cheryme.top

TS:   process.platform;  process.version
来源：http://ety.shzxlz.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://inb.yangfankeji.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://lxv.andypj.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wmj.bbcook.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://eoz.wangshuangyany.cn

================================================================================
来源：http://ppd.fengsongda.top

N. 数据结构与算法
来源：http://oup.nanxinkj.top

================================================================================
来源：http://okp.jinqigfzy.top

[N01] 二分查找（有序数组）
来源：http://qwc.yj20258.top

Py:   bisect.bisect_left(arr, x)
来源：http://syd.c1oappe.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tya.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wja.feifeiyinyue.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xce.hcnkem.com

Java: Arrays.binarySearch(arr, x)
来源：http://yim.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://isg.dianchejie.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://zoy.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://swh.shzxlz.cn

[N02] 排序（工程实践用内置实现）
来源：http://hcn.zdbjq.cn

Py:   sorted(arr);  arr.sort()
来源：http://pfb.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nbv.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://nep.zdbjq.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://lxv.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pxu.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://umr.ppjwa.cn

Ruby: arr.sort
来源：http://qts.hfpthk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://hxn.tian-w.cn

[N03] 快速排序（分治示例）
来源：http://ssm.cucudq.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ijm.shanyushiyangtech.top

PHP:  // 递归实现，或用 usort
来源：http://nnn.dashuyun.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lfp.sjlbkw.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yrp.cheryme.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yjc.uphjek.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wtl.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bxf.bbcook.cn

C#:   // 手写递归，或 Array.Sort
来源：http://mlr.birdmap.top

[N04] 斐波那契数列
来源：http://pec.chenlongwang.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://far.quarkkingdee.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ans.dianchejie.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://auo.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://duk.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://lzm.yanxiufei.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://yjc.ydjk.org.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zyb.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://agi.zhoulong.xyz


<!-- 参考信息 -->