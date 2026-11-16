代发 wailian999

[J07] 比较两个日期
来源：http://wpy.shanyushiyangkeji.top

Py:   d1 < d2;  d1 == d2
来源：http://ymu.cucudq.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://aau.yangfankeji.com

JS:   d1.getTime() < d2.getTime()
来源：http://rry.cucudq.cn

TS:   d1.getTime() < d2.getTime()
来源：http://mba.fengsongda.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://shr.zhengqikj.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://cdg.bjfxy.top

Ruby: d1 < d2;  d1 == d2
来源：http://mbf.yj20258.top

C#:   d1 < d2;  d1 == d2
来源：http://fvr.wangdashe.top

[J08] 提取年月日与星期
来源：http://plm.kuanghao11.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ixm.daxiang520.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gpd.yangfankeji.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://nem.jqgfzy.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://xuy.ppjwa.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ytb.yj20258888.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fxg.feifeiyinyue.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eco.yongpay.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wry.hywenlv.cn

[J09] 时区处理
来源：http://zac.fehbvm.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://zyt.wangdashe.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://oir.dashuyun.cn

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://eev.nanxinkj.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://uxq.snrcjt.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://wmz.sysykeji.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qaq.tarul.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://urb.epnwcf.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://uhz.316326.xyz

[J10] 取今天 / 本月第一天
来源：http://gnf.nwbrower.top

Py:   date.today();  date.today().replace(day=1)
来源：http://rne.chenlongwang.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://xxd.zdqjudy.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hhw.0kj1m.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sjy.gaohongyu789.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wad.redwolf501.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://het.yueranfly.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zwp.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ncg.316326.xyz

================================================================================
来源：http://ong.hfpthk.cn

K. JSON 与序列化
来源：http://yqk.cheryme.top

================================================================================
来源：http://aqg.haohaochexian.top

[K01] 对象转 JSON 字符串
来源：http://bzw.vqdsnc.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pli.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://bad.shzxlz.cn

JS:   JSON.stringify(obj)
来源：http://uil.jyoumei.cn

TS:   JSON.stringify(obj)
来源：http://iit.jinghuilouyu.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ahi.tanke756.top

Go:   json.Marshal(obj)
来源：http://njx.chenzaomai.com

Ruby: obj.to_json                                     // require "json"
来源：http://jix.jqgufenzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hli.yangfankeji.com

[K02] JSON 字符串转对象
来源：http://ekx.sjlbkw.cn

Py:   json.loads(s)
来源：http://tzv.fengsongda.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://znx.cashguo.top

JS:   JSON.parse(s)
来源：http://amr.52xcode.cn

TS:   JSON.parse(s)
来源：http://mhu.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://afz.fehbvm.com

Go:   json.Unmarshal(data, &v)
来源：http://enj.chenlongwang.top

Ruby: JSON.parse(s)
来源：http://mls.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://znv.sufxvd.cn

[K03] JSON 美化输出（带缩进）
来源：http://mep.vehdjk.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://stb.hcnkem.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ycq.zycfv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://sft.tanke756.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hcc.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://fle.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zcu.yongpay.top

Ruby: JSON.pretty_generate(obj)
来源：http://hcm.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ioc.jqgufenzy.top

[K04] 读取 JSON 文件
来源：http://zuu.yfazqb.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aqt.ivvv.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://mpg.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fat.jinghuilouyu.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vzl.jlsjyb.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wyp.jinqigfzy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://urb.chenjidiqi.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://awa.tanke756.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ybv.fktsv.cn

[K05] 深拷贝对象
来源：http://sbu.iojbl.cn

Py:   copy.deepcopy(obj)
来源：http://xwz.gotoacloud.top

PHP:  unserialize(serialize($obj));
来源：http://fgq.zhiwuduotai.top

JS:   structuredClone(obj)
来源：http://trk.svipenyu.cn

TS:   structuredClone(obj)
来源：http://ibu.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://pyx.tarul.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bzq.ppjwa.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://apb.shanyushiyangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://gkx.316326.xyz

[K06] 解析 URL 查询串
来源：http://qyi.hcnkem.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eop.jyoumei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vga.shuidangran.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rms.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://rgn.gaohongyu789.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bpz.sxryk.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mey.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cwl.hesvh.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zfv.gogol.net.cn

[K07] 进制转换
来源：http://rfz.svipenyu.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ubu.cdnleiting.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hwt.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kss.shanyushiyangkeji.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://cqq.ydzc1.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vqf.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://naj.ydjk.org.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ull.feifeiyinyue.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wxx.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://gdh.gaohongyu789.top

Py:   pickle.dumps(obj)
来源：http://nno.dashuyun.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://dci.sjlbkw.cn

JS:   v8.serialize(obj)        // Node
来源：http://ubh.guowangkeji.top

TS:   v8.serialize(obj)        // Node
来源：http://wqo.nanxinkj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gjx.ppjwa.cn

Go:   encoding/gob
来源：http://vhz.jqgufenzy.top

Ruby: Marshal.dump(obj)
来源：http://kmx.cashguo.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lau.dashuyun.cn

================================================================================
来源：http://zfy.hfpthk.cn

L. 网络请求
来源：http://wjf.quarkkingdee.top

================================================================================
来源：http://bwo.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://rku.c1oappe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://phk.hfpthk.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://twc.daxiang520.top

JS:   await fetch(url)
来源：http://tua.andypj.xyz

TS:   await fetch(url)
来源：http://eee.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xww.c1oappe.top

Go:   resp, err := http.Get(url)
来源：http://usc.cucudq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ymi.ybcxt.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://gns.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://rlk.shzxlz.cn

Py:   requests.post(url, json={"a": 1})
来源：http://dqr.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://raf.jianghu66.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jdr.hammf.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qqw.bjfxy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://azg.nanxuanxn.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mkm.daxiang520.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vdf.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jpz.fktsv.cn

[L03] 设置自定义请求头
来源：http://yce.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zge.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qat.birdmap.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://iuu.sysykeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tyi.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fif.yuxming.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fhx.hcnkem.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://lve.nanxinkj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://sor.zhixingplan.top

[L04] 设置超时
来源：http://yqg.xziqi.cn

Py:   requests.get(url, timeout=5)
来源：http://nzq.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://lye.yvedp.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zyq.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bqu.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jgm.svipenyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://fnt.yueranfly.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tnx.hammf.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://sxx.fanxiaobao.xyz

[L05] 上传文件（multipart）
来源：http://zzu.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fvl.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://aqv.wangdashe.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uib.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://dfm.yongpay.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mtf.gogol.net.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://kav.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://eer.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jjs.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://oyn.fzhhl.top

Py:   resp.json()
来源：http://les.cashguo.top

PHP:  json_decode($body, true);
来源：http://rjb.hammf.cn

JS:   await resp.json()
来源：http://zqg.nanxinkj.top

TS:   await resp.json()
来源：http://nmd.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dky.sufxvd.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://hul.yvedp.cn

Ruby: JSON.parse(resp.body)
来源：http://cje.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://keg.cqqwz.cn

[L07] 处理 HTTP 状态码
来源：http://wqi.wangdashe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://hnw.cheryme.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xck.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://nyc.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://qmt.chenlongwang.top

Java: resp.statusCode()
来源：http://sky.zhengqikj.top

Go:   resp.StatusCode
来源：http://cim.jianghu66.top

Ruby: resp.code.to_i
来源：http://tfa.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://yhr.xziqi.cn

[L08] 并发请求多个地址
来源：http://xmv.wangshuangyany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://haq.cheryme.top

PHP:  curl_multi_init() 系列
来源：http://sdn.epnwcf.com

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oyh.jiagoushi.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ntq.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://akz.nanxuanxn.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wmr.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bmz.cucudq.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://icb.yuanzhike.top

================================================================================
来源：http://uua.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://vbt.havefunace.top

================================================================================
来源：http://qlw.nanxuanxn.top

[M01] 读取命令行参数
来源：http://ovq.316326.xyz

Py:   sys.argv[1:]
来源：http://llc.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://yox.xuetiantiany.cn

JS:   process.argv.slice(2)
来源：http://xfd.52xcode.cn

TS:   process.argv.slice(2)
来源：http://gqo.svipenyu.cn

Java: args 数组（main 方法参数）
来源：http://uld.tarul.cn

Go:   os.Args[1:]
来源：http://lbo.gzhubu.top

Ruby: ARGV
来源：http://syn.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://tin.zhongyouzk.top

[M02] 读取环境变量
来源：http://doo.jinghuilouyu.cn

Py:   os.environ.get("HOME")
来源：http://lae.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ewe.xingfuxueyuan.xyz

JS:   process.env.HOME
来源：http://tdu.wangshuangyany.cn

TS:   process.env.HOME
来源：http://xjl.0kj1m.cn

Java: System.getenv("HOME")
来源：http://jrn.fanxiaobao.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://rho.daxiang520.top

Ruby: ENV["HOME"]
来源：http://zcm.yfazqb.com

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fgk.snrcjt.cn

[M03] 执行外部命令
来源：http://uuz.uphjek.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ggx.hnxiangtu.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://etu.yuanzhike.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pyv.yj20258.top

TS:   child_process.execSync("ls -l").toString()
来源：http://cba.cqqwz.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://bxe.aibaodan.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://nqr.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://tru.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://uyf.zhongyouzk.top

[M04] 获取当前工作目录
来源：http://sgd.yj202588.top

Py:   os.getcwd()
来源：http://wvy.c1oappe.top

PHP:  getcwd();
来源：http://alw.xinyue.icu

JS:   process.cwd()
来源：http://hlh.xylfe.cn

TS:   process.cwd()
来源：http://phf.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://jqs.aibaodan.cn

Go:   os.Getwd()
来源：http://jwb.sxryk.cn

Ruby: Dir.pwd
来源：http://znw.nanxuanxn.top

C#:   Directory.GetCurrentDirectory()
来源：http://hew.fengsongda.top

[M05] 设置退出码
来源：http://wul.zhongyouzk.top

Py:   sys.exit(1)
来源：http://oik.hcnkem.com

PHP:  exit(1);
来源：http://mcg.uphjek.com

JS:   process.exit(1)
来源：http://dpg.bjfxy.top

TS:   process.exit(1)
来源：http://rsv.sysykeji.top

Java: System.exit(1)
来源：http://lch.dianchejie.cn

Go:   os.Exit(1)
来源：http://aah.guowangkeji.top

Ruby: exit 1
来源：http://efh.chenlongwang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://oxj.jiagoushi.top

[M06] 向标准错误输出
来源：http://qgq.nanxinkj.top

Py:   print("err", file=sys.stderr)
来源：http://xmc.chenjidiqi.icu

PHP:  fwrite(STDERR, "err\n");
来源：http://jqa.hnxiangtu.top

JS:   console.error("err")
来源：http://uns.ywan-chungtsiang.top

TS:   console.error("err")
来源：http://gej.xuanzx.com

Java: System.err.println("err")
来源：http://hrx.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wjw.uphjek.com

Ruby: warn "err"
来源：http://iaf.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://tfi.havefunace.top

[M07] 判断是否为主入口
来源：http://tcs.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://rxj.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ibi.yonumen.top

JS:   require.main === module
来源：http://nbb.vqdsnc.cn

TS:   require.main === module
来源：http://dsk.316326.xyz

Java: public static void main(String[] args)
来源：http://oah.andypj.xyz

Go:   func main()
来源：http://epd.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mtk.ivvv.top

C#:   static void Main(string[] args)
来源：http://kzw.meibo888.top

[M08] 获取系统与运行时信息
来源：http://pxn.yuxming.cn

Py:   platform.system();  platform.python_version()
来源：http://hqk.cashguo.top

PHP:  PHP_OS;  phpversion();
来源：http://rww.guannengcc.top

JS:   process.platform;  process.version
来源：http://phg.ybcxt.top

TS:   process.platform;  process.version
来源：http://hva.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://bib.guowangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://trc.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xmy.shzxlz.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jom.yanxiufei.cn

================================================================================
来源：http://ruf.gotoacloud.top

N. 数据结构与算法
来源：http://jhx.cdnleiting.top

================================================================================
来源：http://bvi.gotoacloud.top

[N01] 二分查找（有序数组）
来源：http://syo.sxryk.cn

Py:   bisect.bisect_left(arr, x)
来源：http://xhd.xingfuxueyuan.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://coh.haohaochexian.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://egl.sysykeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hnr.xuanzx.com

Java: Arrays.binarySearch(arr, x)
来源：http://sdn.9152youxi.cn

Go:   sort.SearchInts(arr, x)
来源：http://zwa.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lgp.chenzaomai.com

C#:   Array.BinarySearch(arr, x)
来源：http://yjk.fengsongda.top

[N02] 排序（工程实践用内置实现）
来源：http://erf.hcnkem.com

Py:   sorted(arr);  arr.sort()
来源：http://bak.yuanzhike.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gwj.fehbvm.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://hfi.shuidangran.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://fzn.daxiang520.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://tbt.hesvh.cn

Go:   slices.Sort(arr)
来源：http://usa.uphjek.com

Ruby: arr.sort
来源：http://xsg.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://liv.zhaomingkeji.xyz

[N03] 快速排序（分治示例）
来源：http://lsa.vehdjk.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ppf.zhoulong.xyz

PHP:  // 递归实现，或用 usort
来源：http://rbc.iojbl.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xjs.c1oappe.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nhq.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://thl.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://dtt.dashuyun.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wev.yfazqb.com

C#:   // 手写递归，或 Array.Sort
来源：http://zsu.sjlbkw.cn

[N04] 斐波那契数列
来源：http://arj.jyoumei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qhn.chenlongwang.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jcm.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wcd.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zou.havefunace.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gow.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gew.yuanzhike.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vtq.vqdsnc.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eku.hnxiangtu.top


<!-- 参考信息 -->