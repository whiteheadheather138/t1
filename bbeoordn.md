代发 wailian999

[J07] 比较两个日期
来源：http://gbk.nwbrower.top

Py:   d1 < d2;  d1 == d2
来源：http://qzf.tarul.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://kge.jyoumei.cn

JS:   d1.getTime() < d2.getTime()
来源：http://lqu.wangdashe.top

TS:   d1.getTime() < d2.getTime()
来源：http://bfi.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://ktl.hnqzz.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://pvj.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://olk.nwbrower.top

C#:   d1 < d2;  d1 == d2
来源：http://kej.jqgfzy.top

[J08] 提取年月日与星期
来源：http://gjy.xingfuxueyuan.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://srx.tian-w.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dit.smart0.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://cyt.chenjidiqi.icu

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://iui.jqgfzy.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://pca.9152youxi.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ftp.jinqigfzy.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://lfk.9152youxi.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qss.ydjk.org.cn

[J09] 时区处理
来源：http://aua.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://oym.xuanzx.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://cob.tianlin.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mhv.guannengcc.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://syz.shzxlz.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ldn.jinghuilouyu.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://zyl.yfazqb.com

Ruby: Time.now.getlocal("+08:00")
来源：http://fyu.shanyushiyangtech.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ndn.hammf.cn

[J10] 取今天 / 本月第一天
来源：http://bpi.chenjidiqi.icu

Py:   date.today();  date.today().replace(day=1)
来源：http://pjf.wangdashe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://per.xylfe.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nct.fehbvm.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://vxh.hongshengwenyu.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://elt.jqgfzy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gvs.haohaochexian.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nhs.jiagoushi.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://mbs.jlsjyb.cn

================================================================================
来源：http://krc.mhx1999.top

K. JSON 与序列化
来源：http://ltc.aizwys.cn

================================================================================
来源：http://hgi.tanke756.top

[K01] 对象转 JSON 字符串
来源：http://zhh.yanxiufei.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://omt.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jkl.hongshengwenyu.top

JS:   JSON.stringify(obj)
来源：http://ktn.nanxinkj.top

TS:   JSON.stringify(obj)
来源：http://spr.jqgfzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dxt.xinyue.icu

Go:   json.Marshal(obj)
来源：http://dwc.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://paw.yj20258.top

C#:   JsonSerializer.Serialize(obj)
来源：http://sfv.mhx1999.top

[K02] JSON 字符串转对象
来源：http://ueh.xuetiantiany.cn

Py:   json.loads(s)
来源：http://lbf.hfpthk.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://sfk.yanxiufei.cn

JS:   JSON.parse(s)
来源：http://fyg.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://ecq.9152youxi.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jah.shuidangran.top

Go:   json.Unmarshal(data, &v)
来源：http://gxv.sxryk.cn

Ruby: JSON.parse(s)
来源：http://wle.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jhp.gotoacloud.top

[K03] JSON 美化输出（带缩进）
来源：http://akn.yfazqb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sqr.ehwqpu.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://iee.wangshuangyany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://kcl.316326.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://ehg.cucudq.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iis.feifeiyinyue.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://anf.yuxming.cn

Ruby: JSON.pretty_generate(obj)
来源：http://tsy.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yhv.zhijiandao.cn

[K04] 读取 JSON 文件
来源：http://ypx.sxryk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fkm.gaohongyu789.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://wjh.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://bex.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://hrh.9152youxi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jne.gogol.net.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lue.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bhp.zhaomingkeji.xyz

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://uyv.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://npf.aibaodan.cn

Py:   copy.deepcopy(obj)
来源：http://ohb.cdnleiting.top

PHP:  unserialize(serialize($obj));
来源：http://hle.fengsongda.top

JS:   structuredClone(obj)
来源：http://akm.guannengcc.top

TS:   structuredClone(obj)
来源：http://xzi.sysykeji.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lhr.sufxvd.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://nrk.nwbrower.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mdc.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://gac.yvedp.cn

[K06] 解析 URL 查询串
来源：http://hau.xuanzx.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://kwo.fzhhl.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://asf.chenzaomai.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ffr.nwbrower.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nrb.yueranfly.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://qlp.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://wkb.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ywr.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wfy.dianchejie.cn

[K07] 进制转换
来源：http://jlb.quarkkingdee.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dsp.chenzaomai.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nus.dashuyun.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ucp.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://bxy.fzhhl.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lig.nanxinkj.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://keg.yangfankeji.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://plh.hnqzz.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://kcr.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://ere.wangdashe.top

Py:   pickle.dumps(obj)
来源：http://tdi.yuxming.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://sex.c1oappe.top

JS:   v8.serialize(obj)        // Node
来源：http://cmj.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://enc.yueranfly.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://oly.meibo888.top

Go:   encoding/gob
来源：http://ldq.uphjek.com

Ruby: Marshal.dump(obj)
来源：http://pkn.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kbn.sufxvd.cn

================================================================================
来源：http://zfd.andypj.xyz

L. 网络请求
来源：http://emv.cucudq.cn

================================================================================
来源：http://vte.bbcook.cn

[L01] 发送 GET 请求
来源：http://tzi.hongshengwenyu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://yhu.zhixingplan.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://yhf.hywenlv.cn

JS:   await fetch(url)
来源：http://izx.ehwqpu.com

TS:   await fetch(url)
来源：http://olk.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vyh.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://fzn.cqqwz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://wbi.redwolf501.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dhj.ppjwa.cn

[L02] 发送 POST JSON
来源：http://loy.snrcjt.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dgq.feifeiyinyue.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qbq.guowangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://xvj.vqdsnc.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://mjm.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zpb.hammf.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://sdk.mhx1999.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uzr.svipenyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dux.c1oappe.top

[L03] 设置自定义请求头
来源：http://etf.ehwqpu.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lde.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://npo.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vxc.iojbl.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nta.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hev.vehdjk.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://afs.ydjk.org.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://mco.cheryme.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kkv.jiagoushi.top

[L04] 设置超时
来源：http://okl.zhongyouzk.top

Py:   requests.get(url, timeout=5)
来源：http://vfl.zdqjudy.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gkc.mhx1999.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://row.yuxming.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://smn.nwbrower.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://oro.daxiang520.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zwp.wangdashe.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yit.wangdashe.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fvc.ybcxt.top

[L05] 上传文件（multipart）
来源：http://sjj.zdqjudy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lfr.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ifu.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dpx.yongpay.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jqx.zhiwuduotai.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://euh.svipenyu.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fzw.zhoulong.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ous.gzhubu.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wua.sweek.top

[L06] 解析响应为 JSON
来源：http://zxv.yj20258.top

Py:   resp.json()
来源：http://zyr.cashguo.top

PHP:  json_decode($body, true);
来源：http://qbk.shuidangran.top

JS:   await resp.json()
来源：http://jnx.hfpthk.cn

TS:   await resp.json()
来源：http://mme.yvedp.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://baj.jinqigufen.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://sru.jiagoushi.top

Ruby: JSON.parse(resp.body)
来源：http://dnc.yvedp.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pmu.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://nhw.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gzq.gogol.net.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://asc.tian-w.cn

JS:   resp.ok;  resp.status
来源：http://ntg.zhijiandao.cn

TS:   resp.ok;  resp.status
来源：http://oqp.jlsjyb.cn

Java: resp.statusCode()
来源：http://zbd.fengsongda.top

Go:   resp.StatusCode
来源：http://zlq.jinqigfzy.top

Ruby: resp.code.to_i
来源：http://ddl.sufxvd.cn

C#:   (int)resp.StatusCode
来源：http://fvv.aibaodan.cn

[L08] 并发请求多个地址
来源：http://yzi.jinghuilouyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zbx.meibo888.top

PHP:  curl_multi_init() 系列
来源：http://gyx.yuxming.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dmj.ybcxt.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gfv.aibaodan.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vgx.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lpo.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://owo.ctjpmb.com

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fej.cdnleiting.top

================================================================================
来源：http://btn.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://eyr.hfpthk.cn

================================================================================
来源：http://jha.hywenlv.cn

[M01] 读取命令行参数
来源：http://ezp.52xcode.cn

Py:   sys.argv[1:]
来源：http://vec.jqgufenzy.top

PHP:  $argv;  $argc;
来源：http://yat.pycfn.com

JS:   process.argv.slice(2)
来源：http://zph.yuxming.cn

TS:   process.argv.slice(2)
来源：http://tgg.pycfn.com

Java: args 数组（main 方法参数）
来源：http://dud.sysykeji.top

Go:   os.Args[1:]
来源：http://tpm.aibaodan.cn

Ruby: ARGV
来源：http://zkc.epnwcf.com

C#:   args 数组（Main 方法参数）
来源：http://fhj.chenjidiqi.icu

[M02] 读取环境变量
来源：http://eyl.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://bhp.kuanghao11.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://mob.yvedp.cn

JS:   process.env.HOME
来源：http://rnd.jinqigfzy.top

TS:   process.env.HOME
来源：http://kzo.yueranfly.top

Java: System.getenv("HOME")
来源：http://inw.feifeiyinyue.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://thv.snrcjt.cn

Ruby: ENV["HOME"]
来源：http://eiz.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tvi.jiagoushi.top

[M03] 执行外部命令
来源：http://xnd.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fkf.xinyue.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://zfn.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://uhd.shuidangran.top

TS:   child_process.execSync("ls -l").toString()
来源：http://mvy.hfpthk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xsh.guowangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ste.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bgq.yonumen.top

C#:   Process.Start("ls", "-l");
来源：http://tlo.daria6918.cn

[M04] 获取当前工作目录
来源：http://svh.quarkkingdee.top

Py:   os.getcwd()
来源：http://nwm.yongpay.top

PHP:  getcwd();
来源：http://vgp.cdnleiting.top

JS:   process.cwd()
来源：http://pkt.yangfankeji.com

TS:   process.cwd()
来源：http://vkz.birdmap.top

Java: Path.of("").toAbsolutePath()
来源：http://aqm.zhiwuduotai.top

Go:   os.Getwd()
来源：http://cjf.vehdjk.com

Ruby: Dir.pwd
来源：http://owc.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://fsg.yuanzhike.top

[M05] 设置退出码
来源：http://gnl.yj20258888.top

Py:   sys.exit(1)
来源：http://yyq.fzhhl.top

PHP:  exit(1);
来源：http://zjc.yuanzhike.top

JS:   process.exit(1)
来源：http://nxe.cheryme.top

TS:   process.exit(1)
来源：http://ynp.pycfn.com

Java: System.exit(1)
来源：http://wxx.birdmap.top

Go:   os.Exit(1)
来源：http://okf.birdmap.top

Ruby: exit 1
来源：http://jxi.ppjwa.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://hcj.jinqigfzy.top

[M06] 向标准错误输出
来源：http://opw.pycfn.com

Py:   print("err", file=sys.stderr)
来源：http://kyv.hnxiangtu.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gki.fktsv.cn

JS:   console.error("err")
来源：http://vcw.yueranfly.top

TS:   console.error("err")
来源：http://lqn.zhongyouzk.top

Java: System.err.println("err")
来源：http://boy.wangshuangyany.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rmw.smart0.xyz

Ruby: warn "err"
来源：http://fcb.svipenyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://yvg.jinqigfzy.top

[M07] 判断是否为主入口
来源：http://ghs.zhixingplan.top

Py:   if __name__ == "__main__":
来源：http://bbg.snrcjt.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ozd.yuanzhike.top

JS:   require.main === module
来源：http://ixz.bjfxy.top

TS:   require.main === module
来源：http://rex.xuanzx.com

Java: public static void main(String[] args)
来源：http://ydn.yuxming.cn

Go:   func main()
来源：http://ixg.yuanzhike.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ege.ehwqpu.com

C#:   static void Main(string[] args)
来源：http://vzj.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://rjy.hfpthk.cn

Py:   platform.system();  platform.python_version()
来源：http://ztt.chenzaomai.com

PHP:  PHP_OS;  phpversion();
来源：http://skl.316326.xyz

JS:   process.platform;  process.version
来源：http://hsm.hnxiangtu.top

TS:   process.platform;  process.version
来源：http://cas.guowangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://aiy.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://xhn.yueranfly.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://lks.sweek.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://dag.feifeiyinyue.top

================================================================================
来源：http://dbw.quarkkingdee.top

N. 数据结构与算法
来源：http://bqb.cheryme.top

================================================================================
来源：http://lwy.vehdjk.com

[N01] 二分查找（有序数组）
来源：http://wtm.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://xrg.chenzaomai.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lvw.fzhhl.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sxl.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ctx.zhiwuduotai.top

Java: Arrays.binarySearch(arr, x)
来源：http://yvj.yueranfly.top

Go:   sort.SearchInts(arr, x)
来源：http://moa.epnwcf.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://psx.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://nco.pengpengdd.cyou

[N02] 排序（工程实践用内置实现）
来源：http://ilh.fengsongda.top

Py:   sorted(arr);  arr.sort()
来源：http://zqt.zdbjq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://clm.ehwqpu.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://lgh.svipenyu.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jpu.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://lnt.yj20258.top

Go:   slices.Sort(arr)
来源：http://ncj.bjfxy.top

Ruby: arr.sort
来源：http://swz.gogol.net.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://jcw.sxryk.cn

[N03] 快速排序（分治示例）
来源：http://kdy.iojbl.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nyf.feifeiyinyue.top

PHP:  // 递归实现，或用 usort
来源：http://wrt.ehwqpu.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ein.nanxinkj.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jsx.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://wfd.nanxinkj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dsi.quarkkingdee.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://qwy.jqgfzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://kdn.ivvv.top

[N04] 斐波那契数列
来源：http://jla.gaohongyu789.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://caj.snrcjt.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://xra.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ozn.dashuyun.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dsv.mhx1999.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://vpi.chenjidiqi.icu

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://obf.hnqzz.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tia.gogol.net.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ggd.jinyuanbaomall.cn


<!-- 参考信息 -->