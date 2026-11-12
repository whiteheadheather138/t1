代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://ofw.aibaodan.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://jxj.tian-w.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://iwb.jqgufenzy.top

Ruby: d1 < d2;  d1 == d2
来源：http://mkn.yuanzhike.top

C#:   d1 < d2;  d1 == d2
来源：http://grs.fktsv.cn

[J08] 提取年月日与星期
来源：http://yvd.zdqjudy.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://vmq.sufxvd.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://gqe.jinqigfzy.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://msy.havefunace.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://gsw.haohaochexian.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ouc.fanxiaobao.xyz

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://lfk.chenzaomai.com

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://wqb.dianchejie.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://tau.yuxming.cn

[J09] 时区处理
来源：http://htf.tarul.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ljh.shanyushiyangkeji.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://lot.shuidangran.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://abm.jianghu66.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mek.jqgufenzy.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://yxc.kuanghao11.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yln.kuanghao11.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://kwm.tanke756.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://nnl.ydzc1.top

[J10] 取今天 / 本月第一天
来源：http://tuo.gaohongyu789.top

Py:   date.today();  date.today().replace(day=1)
来源：http://wdn.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://dre.xziqi.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://euy.feifeiyinyue.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://xqn.yueranfly.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dfh.yfazqb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qak.hammf.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ffr.cashguo.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://uak.smart0.xyz

================================================================================
来源：http://imj.tianlin.xyz

K. JSON 与序列化
来源：http://idw.redwolf501.top

================================================================================
来源：http://zth.sxryk.cn

[K01] 对象转 JSON 字符串
来源：http://hka.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://asm.bbcook.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kvn.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://okn.ydzc1.top

TS:   JSON.stringify(obj)
来源：http://aad.aibaodan.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ahr.dashuyun.cn

Go:   json.Marshal(obj)
来源：http://fpb.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://iam.52xcode.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://bcl.xuetiantiany.cn

[K02] JSON 字符串转对象
来源：http://jkq.sweek.top

Py:   json.loads(s)
来源：http://dms.nwbrower.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oiv.wangshuangyany.cn

JS:   JSON.parse(s)
来源：http://njc.havefunace.top

TS:   JSON.parse(s)
来源：http://sze.hnqzz.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hfr.fanxiaobao.xyz

Go:   json.Unmarshal(data, &v)
来源：http://nol.dashuyun.cn

Ruby: JSON.parse(s)
来源：http://hqg.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zne.c1oappe.top

[K03] JSON 美化输出（带缩进）
来源：http://owb.ehwqpu.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ljd.yongpay.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://sbb.yuxming.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://yst.zycfv.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://zbf.sjlbkw.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wix.zhengqikj.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jxd.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://wsq.hammf.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iti.nanxinkj.top

[K04] 读取 JSON 文件
来源：http://gqq.nanxinkj.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yps.svipenyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zub.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zsg.haohaochexian.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jkl.zhongyouzk.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vsq.chenzaomai.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://utk.jinqigfzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rcx.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://aqw.gzhubu.top

[K05] 深拷贝对象
来源：http://kun.yfazqb.com

Py:   copy.deepcopy(obj)
来源：http://gmv.jinqigfzy.top

PHP:  unserialize(serialize($obj));
来源：http://ctn.bjfxy.top

JS:   structuredClone(obj)
来源：http://qto.fengsongda.top

TS:   structuredClone(obj)
来源：http://lfs.c1oappe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gdu.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://iqt.fktsv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jrg.ctjpmb.com

C#:   // 序列化往返，或自定义 Clone
来源：http://qyx.cashguo.top

[K06] 解析 URL 查询串
来源：http://rfr.dashuyun.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://zav.hfpthk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jkm.jyoumei.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jis.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ngp.0kj1m.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lqp.xinyue.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://noc.andypj.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mhj.wangdashe.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yyb.jyoumei.cn

[K07] 进制转换
来源：http://jmm.cdnleiting.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cfx.shanyushiyangkeji.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hxa.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yov.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://afv.fktsv.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tiy.sweek.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://edz.fehbvm.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://yph.52xcode.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ocb.yonumen.top

[K08] 二进制序列化（非 JSON）
来源：http://zae.yangfankeji.com

Py:   pickle.dumps(obj)
来源：http://yiw.xuetiantiany.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ofk.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://lxp.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://grp.wangshuangyany.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://bwn.uphjek.com

Go:   encoding/gob
来源：http://ccp.shzxlz.cn

Ruby: Marshal.dump(obj)
来源：http://hyh.sysykeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://opw.shuidangran.top

================================================================================
来源：http://hyk.wangdashe.top

L. 网络请求
来源：http://ubo.gotoacloud.top

================================================================================
来源：http://fuh.fzhhl.top

[L01] 发送 GET 请求
来源：http://sqz.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eul.svipenyu.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fmb.aibaodan.cn

JS:   await fetch(url)
来源：http://apo.jinqigfzy.top

TS:   await fetch(url)
来源：http://ddv.yfazqb.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://sht.xinyue.icu

Go:   resp, err := http.Get(url)
来源：http://irt.316326.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://xhq.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mjs.yuxming.cn

[L02] 发送 POST JSON
来源：http://szm.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://gba.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jrt.nanxinkj.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kwy.shanyushiyangkeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://gei.sweek.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://njt.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://tnq.andypj.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bvn.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mtp.jinghuilouyu.cn

[L03] 设置自定义请求头
来源：http://oqg.zhoulong.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tgm.hfpthk.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dml.ehwqpu.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pku.hnqzz.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hzc.shangyingyoupin.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pvi.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://pbn.gaohongyu789.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://inm.hesvh.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mgg.jinyuanbaomall.cn

[L04] 设置超时
来源：http://sfu.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://rhk.yfazqb.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oby.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gsz.zdbjq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xcp.dianchejie.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ive.iojbl.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vdi.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://htz.ybcxt.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://wol.jinyuanbaomall.cn

[L05] 上传文件（multipart）
来源：http://sfi.zhengqikj.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://imk.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://znc.hongshengwenyu.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nwe.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xiv.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dtx.xuanzx.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jfm.gotoacloud.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://oqc.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hhn.jqgufenzy.top

[L06] 解析响应为 JSON
来源：http://pfg.c1oappe.top

Py:   resp.json()
来源：http://gel.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://tmd.cheryme.top

JS:   await resp.json()
来源：http://opn.guowangkeji.top

TS:   await resp.json()
来源：http://boc.tanke756.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ffp.jinqigfzy.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fal.chenjidiqi.icu

Ruby: JSON.parse(resp.body)
来源：http://xdu.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ocv.pengpengdd.cyou

[L07] 处理 HTTP 状态码
来源：http://byo.zhijiandao.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lof.wangdashe.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://fck.ivvv.top

JS:   resp.ok;  resp.status
来源：http://eum.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://hmm.chenlongwang.top

Java: resp.statusCode()
来源：http://eqy.shuidangran.top

Go:   resp.StatusCode
来源：http://nwq.gzhubu.top

Ruby: resp.code.to_i
来源：http://uce.fanxiaobao.xyz

C#:   (int)resp.StatusCode
来源：http://bsr.sjlbkw.cn

[L08] 并发请求多个地址
来源：http://rna.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kvo.dashuyun.cn

PHP:  curl_multi_init() 系列
来源：http://ves.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mrt.zhoulong.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kcr.dianchejie.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://yyd.redwolf501.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pqo.jinqigufen.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://zoi.ydjk.org.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://lsx.jlsjyb.cn

================================================================================
来源：http://qam.zhijiandao.cn

M. 命令行 / 进程 / 环境
来源：http://fqr.andypj.xyz

================================================================================
来源：http://zzj.chenjidiqi.icu

[M01] 读取命令行参数
来源：http://gbm.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://pbx.chenzaomai.com

PHP:  $argv;  $argc;
来源：http://dmd.jinyuanbaomall.cn

JS:   process.argv.slice(2)
来源：http://yca.jyoumei.cn

TS:   process.argv.slice(2)
来源：http://yfj.pycfn.com

Java: args 数组（main 方法参数）
来源：http://mvn.gaohongyu789.top

Go:   os.Args[1:]
来源：http://anl.shzxlz.cn

Ruby: ARGV
来源：http://vtm.yanxiufei.cn

C#:   args 数组（Main 方法参数）
来源：http://flu.feifeiyinyue.top

[M02] 读取环境变量
来源：http://nuh.ppjwa.cn

Py:   os.environ.get("HOME")
来源：http://nmz.aibaodan.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://yrk.dianchejie.cn

JS:   process.env.HOME
来源：http://xho.hywenlv.cn

TS:   process.env.HOME
来源：http://ofh.xziqi.cn

Java: System.getenv("HOME")
来源：http://xbg.zhongyouzk.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vcr.jyoumei.cn

Ruby: ENV["HOME"]
来源：http://zoh.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://rwr.shanyushiyangkeji.top

[M03] 执行外部命令
来源：http://unu.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://cfx.daxiang520.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wfx.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ulr.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lmp.wangdashe.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kwv.jqgfzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://uzg.9152youxi.cn

Ruby: system("ls -l");  `ls -l`
来源：http://qeq.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://acl.zhixingplan.top

[M04] 获取当前工作目录
来源：http://clt.hongshengwenyu.top

Py:   os.getcwd()
来源：http://xzl.zhixingplan.top

PHP:  getcwd();
来源：http://pbr.hesvh.cn

JS:   process.cwd()
来源：http://dsp.jqgfzy.top

TS:   process.cwd()
来源：http://lyd.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://kaj.snrcjt.cn

Go:   os.Getwd()
来源：http://bhh.gaohongyu789.top

Ruby: Dir.pwd
来源：http://jaw.guannengcc.top

C#:   Directory.GetCurrentDirectory()
来源：http://llh.guannengcc.top

[M05] 设置退出码
来源：http://jyd.gzhubu.top

Py:   sys.exit(1)
来源：http://qun.cheryme.top

PHP:  exit(1);
来源：http://thb.wangshuangyany.cn

JS:   process.exit(1)
来源：http://sdd.yj20258888.top

TS:   process.exit(1)
来源：http://foi.hongshengwenyu.top

Java: System.exit(1)
来源：http://aov.sufxvd.cn

Go:   os.Exit(1)
来源：http://nmq.bjfxy.top

Ruby: exit 1
来源：http://vkh.guannengcc.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bva.feifeiyinyue.top

[M06] 向标准错误输出
来源：http://hxg.wangshuangyany.cn

Py:   print("err", file=sys.stderr)
来源：http://dzf.hesvh.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nqe.ydzc1.top

JS:   console.error("err")
来源：http://dqz.bjfxy.top

TS:   console.error("err")
来源：http://dbv.fengsongda.top

Java: System.err.println("err")
来源：http://ops.shanyushiyangtech.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hpr.yueranfly.top

Ruby: warn "err"
来源：http://kyx.shanyushiyangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://rbg.shanyushiyangkeji.top

[M07] 判断是否为主入口
来源：http://ufb.cucudq.cn

Py:   if __name__ == "__main__":
来源：http://myk.xingfuxueyuan.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://izm.xinyue.icu

JS:   require.main === module
来源：http://lle.chenjidiqi.icu

TS:   require.main === module
来源：http://xpv.jinyuanbaomall.cn

Java: public static void main(String[] args)
来源：http://hwd.jinqigfzy.top

Go:   func main()
来源：http://mmo.hywenlv.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://swu.tarul.cn

C#:   static void Main(string[] args)
来源：http://cce.mhx1999.top

[M08] 获取系统与运行时信息
来源：http://pko.hammf.cn

Py:   platform.system();  platform.python_version()
来源：http://xpr.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://ykm.ywan-chungtsiang.top

JS:   process.platform;  process.version
来源：http://kkg.hcnkem.com

TS:   process.platform;  process.version
来源：http://sth.yuxming.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kwo.c1oappe.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ust.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fpp.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://nau.epnwcf.com

================================================================================
来源：http://wpa.quarkkingdee.top

N. 数据结构与算法
来源：http://gvo.cqqwz.cn

================================================================================
来源：http://wme.xziqi.cn

[N01] 二分查找（有序数组）
来源：http://uek.chenlongwang.top

Py:   bisect.bisect_left(arr, x)
来源：http://rvu.haohaochexian.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nfg.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ora.cheryme.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vbb.sysykeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://rdv.shanyushiyangkeji.top

Go:   sort.SearchInts(arr, x)
来源：http://duh.nanxinkj.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://vbq.ydzc1.top

C#:   Array.BinarySearch(arr, x)
来源：http://mus.xuetiantiany.cn

[N02] 排序（工程实践用内置实现）
来源：http://gro.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://rka.ydzc1.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://raz.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ibg.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://mai.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cpm.zdqjudy.top

Go:   slices.Sort(arr)
来源：http://cwc.shuidangran.top

Ruby: arr.sort
来源：http://hfl.hcnkem.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://xhu.jinyuanbaomall.cn

[N03] 快速排序（分治示例）
来源：http://oqr.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hki.gzhubu.top

PHP:  // 递归实现，或用 usort
来源：http://wcf.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kxf.zycfv.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jrh.nanxinkj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://rye.pengpengdd.cyou

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ued.jiagoushi.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://yfu.xinyue.icu

C#:   // 手写递归，或 Array.Sort
来源：http://atb.cashguo.top

[N04] 斐波那契数列
来源：http://cbj.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://crf.xinyue.icu

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://igl.guannengcc.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://uvy.ywan-chungtsiang.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kfj.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bty.smart0.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hvk.yj202588.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kib.guannengcc.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://oqn.vqdsnc.cn

[N05] 最大公约数
来源：http://dpx.tian-w.cn

Py:   math.gcd(a, b)
来源：http://yvu.havefunace.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qdx.cheryme.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gcj.zhixingplan.top


<!-- 参考信息 -->