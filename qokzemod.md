代发 wailian999

[J07] 比较两个日期
来源：http://vmm.daxiang520.top

Py:   d1 < d2;  d1 == d2
来源：http://hvo.316326.xyz

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://obz.yfazqb.com

JS:   d1.getTime() < d2.getTime()
来源：http://dth.pengpengdd.cyou

TS:   d1.getTime() < d2.getTime()
来源：http://ekq.0kj1m.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ypi.cashguo.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://uym.sweek.top

Ruby: d1 < d2;  d1 == d2
来源：http://tir.bbcook.cn

C#:   d1 < d2;  d1 == d2
来源：http://iae.zhijiandao.cn

[J08] 提取年月日与星期
来源：http://pda.c1oappe.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://xwd.shangyingyoupin.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ujp.ctjpmb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://ewu.daxiang520.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://ydp.hnqzz.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://odz.fengsongda.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://uag.yj20258888.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fzk.jinqigfzy.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://evw.epnwcf.com

[J09] 时区处理
来源：http://jua.shanyushiyangtech.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://obw.hywenlv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bli.shanyushiyangtech.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xxw.zhiwuduotai.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://dnl.ydzc1.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://tya.yfazqb.com

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qze.dianchejie.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vsw.quarkkingdee.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jsf.ehwqpu.com

[J10] 取今天 / 本月第一天
来源：http://tei.xinyue.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://mbu.nanxuanxn.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eju.yuxming.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://iax.yj20258888.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://onh.nwbrower.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lnh.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://izb.jqgufenzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vsi.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://tah.zdqjudy.top

================================================================================
来源：http://bcm.hongshengwenyu.top

K. JSON 与序列化
来源：http://ksb.shuidangran.top

================================================================================
来源：http://fhc.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://usd.andypj.xyz

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fed.guowangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://uji.jianghu66.top

JS:   JSON.stringify(obj)
来源：http://kwo.cheryme.top

TS:   JSON.stringify(obj)
来源：http://vun.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dmc.chenjidiqi.icu

Go:   json.Marshal(obj)
来源：http://lbd.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://rwi.hysaishi.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bdd.hcnkem.com

[K02] JSON 字符串转对象
来源：http://yjs.tarul.cn

Py:   json.loads(s)
来源：http://njz.yj20258888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sqe.yj20258.top

JS:   JSON.parse(s)
来源：http://ogk.smart0.xyz

TS:   JSON.parse(s)
来源：http://jpn.vqdsnc.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://agq.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://jid.nanxinkj.top

Ruby: JSON.parse(s)
来源：http://ytk.jyoumei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bbd.zhiwuduotai.top

[K03] JSON 美化输出（带缩进）
来源：http://lwe.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wiv.chenjidiqi.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://syz.jyoumei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://fua.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://fzx.zhiwuduotai.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://zsh.pycfn.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pal.sxryk.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tkb.ehwqpu.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ckw.hywenlv.cn

[K04] 读取 JSON 文件
来源：http://gpd.bbcook.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://age.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://bvv.fehbvm.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://eqo.hnxiangtu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zfh.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://svd.jinghuilouyu.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://nkx.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://ucs.yonumen.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://wgt.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://pay.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://dxi.sjlbkw.cn

PHP:  unserialize(serialize($obj));
来源：http://uau.bbcook.cn

JS:   structuredClone(obj)
来源：http://sdf.shanyushiyangtech.top

TS:   structuredClone(obj)
来源：http://hit.xuanzx.com

Java: // 手写拷贝构造，或序列化往返
来源：http://fwb.quarkkingdee.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://yqn.yj20258.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tbm.quarkkingdee.top

C#:   // 序列化往返，或自定义 Clone
来源：http://egb.c1oappe.top

[K06] 解析 URL 查询串
来源：http://omb.jiagoushi.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://rnf.chenlongwang.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ddr.52xcode.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hzc.ydzc1.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hyg.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://usv.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://amu.fzhhl.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cht.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xmf.yj202588.top

[K07] 进制转换
来源：http://afu.meibo888.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ese.xylfe.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zgh.pengpengdd.cyou

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zpf.jinyuanbaomall.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://uhm.feifeiyinyue.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://zwf.zhijiandao.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://nzj.hysaishi.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zlk.zhongyouzk.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://odj.meibo888.top

[K08] 二进制序列化（非 JSON）
来源：http://ytz.c1oappe.top

Py:   pickle.dumps(obj)
来源：http://emi.ehwqpu.com

PHP:  serialize($obj);  unserialize($s);
来源：http://npj.yfazqb.com

JS:   v8.serialize(obj)        // Node
来源：http://wkd.pengpengdd.cyou

TS:   v8.serialize(obj)        // Node
来源：http://hqr.bjfxy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fhx.xziqi.cn

Go:   encoding/gob
来源：http://sdt.xuanzx.com

Ruby: Marshal.dump(obj)
来源：http://tuq.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://erw.cashguo.top

================================================================================
来源：http://uwo.hcnkem.com

L. 网络请求
来源：http://geb.shangyingyoupin.top

================================================================================
来源：http://xzr.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://ald.gaohongyu789.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nno.vehdjk.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qrq.jiagoushi.top

JS:   await fetch(url)
来源：http://hcv.hywenlv.cn

TS:   await fetch(url)
来源：http://vlp.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pdp.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://xsi.dianchejie.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://stb.snrcjt.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://pip.tian-w.cn

[L02] 发送 POST JSON
来源：http://xwh.jinghuilouyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://kvn.guannengcc.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://dhp.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pmu.ehwqpu.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ffg.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qmx.yanxiufei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://haj.hammf.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uan.yongpay.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://lat.gotoacloud.top

[L03] 设置自定义请求头
来源：http://kxx.redwolf501.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vvo.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://hnu.bbcook.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hqa.jinyuanbaomall.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wjv.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://vzl.yj202588.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ugg.daxiang520.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://stq.ybcxt.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tvk.ctjpmb.com

[L04] 设置超时
来源：http://bok.yongpay.top

Py:   requests.get(url, timeout=5)
来源：http://rfd.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mfx.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jso.havefunace.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rbb.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://buh.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xzd.hammf.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://uul.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://via.hysaishi.cn

[L05] 上传文件（multipart）
来源：http://nnb.aibaodan.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://toi.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mxc.aizwys.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qtt.wangdashe.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://zgv.chenjidiqi.icu

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ote.ppjwa.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kmh.jiagoushi.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xog.chenlongwang.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ebn.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://sjg.yuanzhike.top

Py:   resp.json()
来源：http://kor.shuidangran.top

PHP:  json_decode($body, true);
来源：http://baz.yangfankeji.com

JS:   await resp.json()
来源：http://yuh.yvedp.cn

TS:   await resp.json()
来源：http://isb.iojbl.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://pzu.sweek.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hox.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://mvq.vqdsnc.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cao.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://pgt.yj20258888.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hbd.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qsr.jinyuanbaomall.cn

JS:   resp.ok;  resp.status
来源：http://blb.zhongyouzk.top

TS:   resp.ok;  resp.status
来源：http://sdb.xuanzx.com

Java: resp.statusCode()
来源：http://qzf.bjfxy.top

Go:   resp.StatusCode
来源：http://iuz.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://cqw.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://qcx.shanyushiyangkeji.top

[L08] 并发请求多个地址
来源：http://vdt.jianghu66.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ekw.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://lrx.zhongyouzk.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://adv.hfpthk.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ttc.jinyuanbaomall.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kvn.andypj.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ybi.jinqigfzy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cyt.shanyushiyangkeji.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://avr.guannengcc.top

================================================================================
来源：http://dmi.jlsjyb.cn

M. 命令行 / 进程 / 环境
来源：http://yks.sufxvd.cn

================================================================================
来源：http://lqc.zhijiandao.cn

[M01] 读取命令行参数
来源：http://mlq.cqqwz.cn

Py:   sys.argv[1:]
来源：http://ddr.jyoumei.cn

PHP:  $argv;  $argc;
来源：http://rms.ehwqpu.com

JS:   process.argv.slice(2)
来源：http://wkp.hfpthk.cn

TS:   process.argv.slice(2)
来源：http://pgd.ybcxt.top

Java: args 数组（main 方法参数）
来源：http://wwy.aibaodan.cn

Go:   os.Args[1:]
来源：http://oyf.havefunace.top

Ruby: ARGV
来源：http://nif.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://yut.0kj1m.cn

[M02] 读取环境变量
来源：http://hoo.snrcjt.cn

Py:   os.environ.get("HOME")
来源：http://vlx.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ggy.nanxinkj.top

JS:   process.env.HOME
来源：http://lvw.cheryme.top

TS:   process.env.HOME
来源：http://xpm.0kj1m.cn

Java: System.getenv("HOME")
来源：http://kqx.cqqwz.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://hms.xziqi.cn

Ruby: ENV["HOME"]
来源：http://ter.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xgh.smart0.xyz

[M03] 执行外部命令
来源：http://sma.jinyuanbaomall.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fni.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wkd.shanyushiyangtech.top

JS:   child_process.execSync("ls -l").toString()
来源：http://efx.smart0.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://bkg.aizwys.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fyn.c1oappe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nru.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://syi.wangdashe.top

C#:   Process.Start("ls", "-l");
来源：http://iui.0kj1m.cn

[M04] 获取当前工作目录
来源：http://stc.vqdsnc.cn

Py:   os.getcwd()
来源：http://pqb.hongshengwenyu.top

PHP:  getcwd();
来源：http://vxk.hnxiangtu.top

JS:   process.cwd()
来源：http://tlm.feifeiyinyue.top

TS:   process.cwd()
来源：http://ogh.dianchejie.cn

Java: Path.of("").toAbsolutePath()
来源：http://qbl.zycfv.cn

Go:   os.Getwd()
来源：http://wdx.quarkkingdee.top

Ruby: Dir.pwd
来源：http://lfa.tarul.cn

C#:   Directory.GetCurrentDirectory()
来源：http://gep.xuetiantiany.cn

[M05] 设置退出码
来源：http://stn.ivvv.top

Py:   sys.exit(1)
来源：http://auy.cucudq.cn

PHP:  exit(1);
来源：http://xux.zhaomingkeji.xyz

JS:   process.exit(1)
来源：http://zbr.cashguo.top

TS:   process.exit(1)
来源：http://rms.guannengcc.top

Java: System.exit(1)
来源：http://gei.zhaomingkeji.xyz

Go:   os.Exit(1)
来源：http://bbx.tian-w.cn

Ruby: exit 1
来源：http://kdx.sxryk.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ywv.sysykeji.top

[M06] 向标准错误输出
来源：http://dto.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://qmt.yanxiufei.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://jem.fzhhl.top

JS:   console.error("err")
来源：http://ckr.quarkkingdee.top

TS:   console.error("err")
来源：http://hkp.kuanghao11.cn

Java: System.err.println("err")
来源：http://vsv.aizwys.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://uya.wangdashe.top

Ruby: warn "err"
来源：http://tfs.yongpay.top

C#:   Console.Error.WriteLine("err")
来源：http://hxk.vqdsnc.cn

[M07] 判断是否为主入口
来源：http://mla.jinqigufen.top

Py:   if __name__ == "__main__":
来源：http://ajb.tianlin.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jej.fktsv.cn

JS:   require.main === module
来源：http://pbu.ppjwa.cn

TS:   require.main === module
来源：http://obi.jlsjyb.cn

Java: public static void main(String[] args)
来源：http://xbp.nanxinkj.top

Go:   func main()
来源：http://yhq.yj20258.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dqf.yvedp.cn

C#:   static void Main(string[] args)
来源：http://iug.zhixingplan.top

[M08] 获取系统与运行时信息
来源：http://sew.fzhhl.top

Py:   platform.system();  platform.python_version()
来源：http://mln.ydjk.org.cn

PHP:  PHP_OS;  phpversion();
来源：http://szi.sweek.top

JS:   process.platform;  process.version
来源：http://wuf.shanyushiyangkeji.top

TS:   process.platform;  process.version
来源：http://dnd.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qam.nwbrower.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sbi.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wsq.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://axw.pycfn.com

================================================================================
来源：http://llt.feifeiyinyue.top

N. 数据结构与算法
来源：http://lje.epnwcf.com

================================================================================
来源：http://vyx.fzhhl.top

[N01] 二分查找（有序数组）
来源：http://ydz.shangyingyoupin.top

Py:   bisect.bisect_left(arr, x)
来源：http://qel.hongshengwenyu.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aqd.jiagoushi.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sry.jyoumei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://fbb.jyoumei.cn

Java: Arrays.binarySearch(arr, x)
来源：http://olz.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://kqv.chenjidiqi.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://jqm.shuidangran.top

C#:   Array.BinarySearch(arr, x)
来源：http://sxv.hnqzz.top

[N02] 排序（工程实践用内置实现）
来源：http://jpm.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://aek.zdqjudy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qqm.guannengcc.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://cqm.fengsongda.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://pcr.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dhm.pycfn.com

Go:   slices.Sort(arr)
来源：http://aht.hywenlv.cn

Ruby: arr.sort
来源：http://dhx.fehbvm.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://lnx.sufxvd.cn

[N03] 快速排序（分治示例）
来源：http://dgz.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rwa.xziqi.cn

PHP:  // 递归实现，或用 usort
来源：http://vts.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lsl.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rjz.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nya.tianlin.xyz

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mim.redwolf501.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jei.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://ywi.bbcook.cn

[N04] 斐波那契数列
来源：http://eiy.tarul.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rst.hammf.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://efy.dashuyun.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eqj.ybcxt.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cwy.wangshuangyany.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dfp.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mof.shzxlz.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fzb.daria6918.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ojf.aibaodan.cn


<!-- 参考信息 -->