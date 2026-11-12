代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://wdq.guowangkeji.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://iox.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://tgq.ydzc1.top

Ruby: d1 < d2;  d1 == d2
来源：http://jdz.sysykeji.top

C#:   d1 < d2;  d1 == d2
来源：http://jdq.jqgufenzy.top

[J08] 提取年月日与星期
来源：http://ved.hammf.cn

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hku.vqdsnc.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://pkf.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://dtj.nwbrower.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://srn.yfazqb.com

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://yfz.wangshuangyany.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://zmc.zhiwuduotai.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://zlb.epnwcf.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://whc.redwolf501.top

[J09] 时区处理
来源：http://pss.uphjek.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hon.zhoulong.xyz

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://qrq.hcnkem.com

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://bne.tarul.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://qpx.iojbl.cn

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://lkk.meibo888.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://thy.daxiang520.top

Ruby: Time.now.getlocal("+08:00")
来源：http://hxq.svipenyu.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oag.hysaishi.cn

[J10] 取今天 / 本月第一天
来源：http://uxw.dianchejie.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://tja.sweek.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://eib.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://ruv.shanyushiyangkeji.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://zcy.fengsongda.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://scr.kuanghao11.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://uls.uphjek.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://wyr.xziqi.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qyx.tanke756.top

================================================================================
来源：http://eit.cqqwz.cn

K. JSON 与序列化
来源：http://jby.ppjwa.cn

================================================================================
来源：http://blw.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://mju.cashguo.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://nqf.yfazqb.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dep.gogol.net.cn

JS:   JSON.stringify(obj)
来源：http://ape.zhixingplan.top

TS:   JSON.stringify(obj)
来源：http://wbq.cucudq.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jfo.feifeiyinyue.top

Go:   json.Marshal(obj)
来源：http://wdp.jianghu66.top

Ruby: obj.to_json                                     // require "json"
来源：http://suk.jinqigufen.top

C#:   JsonSerializer.Serialize(obj)
来源：http://xan.jinghuilouyu.cn

[K02] JSON 字符串转对象
来源：http://nze.shanyushiyangkeji.top

Py:   json.loads(s)
来源：http://eop.svipenyu.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://etn.fktsv.cn

JS:   JSON.parse(s)
来源：http://qld.jinyuanbaomall.cn

TS:   JSON.parse(s)
来源：http://nhe.xylfe.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pij.cqqwz.cn

Go:   json.Unmarshal(data, &v)
来源：http://mla.zhaomingkeji.xyz

Ruby: JSON.parse(s)
来源：http://bqd.sweek.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ugd.yongpay.top

[K03] JSON 美化输出（带缩进）
来源：http://czz.sweek.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uia.kuanghao11.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://huj.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://odc.c1oappe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://gum.chenjidiqi.icu

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://wfv.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cjm.wangdashe.top

Ruby: JSON.pretty_generate(obj)
来源：http://cds.mhx1999.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://shd.tanke756.top

[K04] 读取 JSON 文件
来源：http://fuq.ppjwa.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://pdb.zycfv.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://lkq.tarul.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://poz.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rby.hcnkem.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ppy.wangshuangyany.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ras.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://vcy.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mgb.pengpengdd.cyou

[K05] 深拷贝对象
来源：http://kwz.cdnleiting.top

Py:   copy.deepcopy(obj)
来源：http://pyz.dianchejie.cn

PHP:  unserialize(serialize($obj));
来源：http://bvo.yonumen.top

JS:   structuredClone(obj)
来源：http://dqz.zdbjq.cn

TS:   structuredClone(obj)
来源：http://ahn.sjlbkw.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nqy.hongshengwenyu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qjg.yonumen.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wqb.wangdashe.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nwk.ydjk.org.cn

[K06] 解析 URL 查询串
来源：http://bcs.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://win.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wlk.smart0.xyz

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lsj.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pns.xylfe.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dbx.daria6918.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qhc.yfazqb.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tfh.bjfxy.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://bnv.shzxlz.cn

[K07] 进制转换
来源：http://tdp.pycfn.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://myd.zhijiandao.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nzy.andypj.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pms.zhixingplan.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://hnt.sufxvd.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qey.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://yyt.smart0.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://exe.yueranfly.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jss.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://pbj.fehbvm.com

Py:   pickle.dumps(obj)
来源：http://pnp.shanyushiyangkeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://bva.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://dwi.hywenlv.cn

TS:   v8.serialize(obj)        // Node
来源：http://ale.zhengqikj.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hlb.gotoacloud.top

Go:   encoding/gob
来源：http://vml.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://dry.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lex.cdnleiting.top

================================================================================
来源：http://wsn.nanxuanxn.top

L. 网络请求
来源：http://muz.shanyushiyangtech.top

================================================================================
来源：http://uep.tian-w.cn

[L01] 发送 GET 请求
来源：http://iwk.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rmm.yanxiufei.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bpq.jiagoushi.top

JS:   await fetch(url)
来源：http://hyj.xziqi.cn

TS:   await fetch(url)
来源：http://ksi.xingfuxueyuan.xyz

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wrh.yonumen.top

Go:   resp, err := http.Get(url)
来源：http://rma.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fdx.chenzaomai.com

C#:   await new HttpClient().GetStringAsync(url)
来源：http://rng.gogol.net.cn

[L02] 发送 POST JSON
来源：http://mzi.sweek.top

Py:   requests.post(url, json={"a": 1})
来源：http://eip.jlsjyb.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://qyz.guowangkeji.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ivf.fzhhl.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dji.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://orn.zycfv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rsq.shzxlz.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fky.zhoulong.xyz

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pyr.shanyushiyangkeji.top

[L03] 设置自定义请求头
来源：http://cwt.xuetiantiany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jtx.fzhhl.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://bow.xuetiantiany.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zrt.zhijiandao.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tgp.jinyuanbaomall.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qfq.shuidangran.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://bno.hfpthk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://baz.redwolf501.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tjj.pengpengdd.cyou

[L04] 设置超时
来源：http://xmm.bbcook.cn

Py:   requests.get(url, timeout=5)
来源：http://dqf.jinghuilouyu.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://mwn.ybcxt.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fje.yonumen.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bmf.52xcode.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ziy.ctjpmb.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bus.daria6918.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xmr.meibo888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ehk.aibaodan.cn

[L05] 上传文件（multipart）
来源：http://dyz.gotoacloud.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mhy.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://hbh.52xcode.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uih.hammf.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tkc.shangyingyoupin.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://oai.yanxiufei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://isp.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uuc.sysykeji.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kyc.dianchejie.cn

[L06] 解析响应为 JSON
来源：http://yec.cheryme.top

Py:   resp.json()
来源：http://ypx.yj20258.top

PHP:  json_decode($body, true);
来源：http://fln.tianlin.xyz

JS:   await resp.json()
来源：http://ebk.zhongyouzk.top

TS:   await resp.json()
来源：http://vlg.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bjd.dashuyun.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kqb.cashguo.top

Ruby: JSON.parse(resp.body)
来源：http://rto.52xcode.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ssj.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://ouv.ydzc1.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zkq.guowangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ivj.xingfuxueyuan.xyz

JS:   resp.ok;  resp.status
来源：http://iop.bjfxy.top

TS:   resp.ok;  resp.status
来源：http://igh.epnwcf.com

Java: resp.statusCode()
来源：http://jgm.zhixingplan.top

Go:   resp.StatusCode
来源：http://uns.wangdashe.top

Ruby: resp.code.to_i
来源：http://lyg.chenjidiqi.icu

C#:   (int)resp.StatusCode
来源：http://iqb.ehwqpu.com

[L08] 并发请求多个地址
来源：http://gaj.sweek.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tuh.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://cxe.xziqi.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rrx.ydzc1.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vfs.fanxiaobao.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://kdc.gzhubu.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qrv.yj20258.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rtv.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://dhj.bjfxy.top

================================================================================
来源：http://woo.jinqigfzy.top

M. 命令行 / 进程 / 环境
来源：http://qwf.kuanghao11.cn

================================================================================
来源：http://uyi.ivvv.top

[M01] 读取命令行参数
来源：http://mwq.ppjwa.cn

Py:   sys.argv[1:]
来源：http://vbw.hnqzz.top

PHP:  $argv;  $argc;
来源：http://qgx.hesvh.cn

JS:   process.argv.slice(2)
来源：http://wpl.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://wcz.cqqwz.cn

Java: args 数组（main 方法参数）
来源：http://wor.pengpengdd.cyou

Go:   os.Args[1:]
来源：http://lja.hnqzz.top

Ruby: ARGV
来源：http://upz.sysykeji.top

C#:   args 数组（Main 方法参数）
来源：http://pcp.svipenyu.cn

[M02] 读取环境变量
来源：http://wpn.daxiang520.top

Py:   os.environ.get("HOME")
来源：http://pwj.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://scx.yfazqb.com

JS:   process.env.HOME
来源：http://fxu.gotoacloud.top

TS:   process.env.HOME
来源：http://oda.c1oappe.top

Java: System.getenv("HOME")
来源：http://tde.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gww.nanxinkj.top

Ruby: ENV["HOME"]
来源：http://sxa.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://pqq.hfpthk.cn

[M03] 执行外部命令
来源：http://uei.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://spx.vqdsnc.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qnx.yongpay.top

JS:   child_process.execSync("ls -l").toString()
来源：http://pse.shzxlz.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://spb.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wqw.cqqwz.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://lqw.shanyushiyangkeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://hds.uphjek.com

C#:   Process.Start("ls", "-l");
来源：http://hkc.pengpengdd.cyou

[M04] 获取当前工作目录
来源：http://vca.fzhhl.top

Py:   os.getcwd()
来源：http://zvo.9152youxi.cn

PHP:  getcwd();
来源：http://jfv.sxryk.cn

JS:   process.cwd()
来源：http://rpd.sxryk.cn

TS:   process.cwd()
来源：http://mwo.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://uoa.ydjk.org.cn

Go:   os.Getwd()
来源：http://ryw.tanke756.top

Ruby: Dir.pwd
来源：http://osc.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://fbs.yueranfly.top

[M05] 设置退出码
来源：http://pkf.xylfe.cn

Py:   sys.exit(1)
来源：http://gqu.sxryk.cn

PHP:  exit(1);
来源：http://hrf.zhijiandao.cn

JS:   process.exit(1)
来源：http://ycp.jinqigfzy.top

TS:   process.exit(1)
来源：http://rhi.hongshengwenyu.top

Java: System.exit(1)
来源：http://flo.andypj.xyz

Go:   os.Exit(1)
来源：http://whm.chenzaomai.com

Ruby: exit 1
来源：http://gqw.wangshuangyany.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uoy.hfpthk.cn

[M06] 向标准错误输出
来源：http://qui.jyoumei.cn

Py:   print("err", file=sys.stderr)
来源：http://mjf.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ums.ybcxt.top

JS:   console.error("err")
来源：http://ief.xuanzx.com

TS:   console.error("err")
来源：http://aue.zhongyouzk.top

Java: System.err.println("err")
来源：http://mwq.sysykeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hvl.andypj.xyz

Ruby: warn "err"
来源：http://dlw.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://chr.zhoulong.xyz

[M07] 判断是否为主入口
来源：http://qpn.jlsjyb.cn

Py:   if __name__ == "__main__":
来源：http://kre.zhixingplan.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://nwe.jianghu66.top

JS:   require.main === module
来源：http://gge.9152youxi.cn

TS:   require.main === module
来源：http://diz.uphjek.com

Java: public static void main(String[] args)
来源：http://vrr.zdbjq.cn

Go:   func main()
来源：http://ohj.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tjw.fzhhl.top

C#:   static void Main(string[] args)
来源：http://jpi.sjlbkw.cn

[M08] 获取系统与运行时信息
来源：http://ijk.smart0.xyz

Py:   platform.system();  platform.python_version()
来源：http://trb.jyoumei.cn

PHP:  PHP_OS;  phpversion();
来源：http://eka.hesvh.cn

JS:   process.platform;  process.version
来源：http://qoc.zdqjudy.top

TS:   process.platform;  process.version
来源：http://ckq.daxiang520.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://egp.ppjwa.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://atk.nwbrower.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xph.cheryme.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://gtj.vqdsnc.cn

================================================================================
来源：http://eqg.xuetiantiany.cn

N. 数据结构与算法
来源：http://tur.jinyuanbaomall.cn

================================================================================
来源：http://jti.sysykeji.top

[N01] 二分查找（有序数组）
来源：http://csl.cucudq.cn

Py:   bisect.bisect_left(arr, x)
来源：http://enk.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hsn.xuanzx.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://adj.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gqb.jinqigfzy.top

Java: Arrays.binarySearch(arr, x)
来源：http://fkr.sweek.top

Go:   sort.SearchInts(arr, x)
来源：http://eyv.ydzc1.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://bpn.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://nur.zhixingplan.top

[N02] 排序（工程实践用内置实现）
来源：http://zoh.yuxming.cn

Py:   sorted(arr);  arr.sort()
来源：http://spg.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sss.jyoumei.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://ghf.zhaomingkeji.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://cuk.zdqjudy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qtd.meibo888.top

Go:   slices.Sort(arr)
来源：http://ycv.hfpthk.cn

Ruby: arr.sort
来源：http://vsm.zhoulong.xyz

C#:   Array.Sort(arr);  list.Sort()
来源：http://ags.yueranfly.top

[N03] 快速排序（分治示例）
来源：http://vwa.zhoulong.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://hsp.snrcjt.cn

PHP:  // 递归实现，或用 usort
来源：http://nxy.xziqi.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://wrj.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hxn.shanyushiyangkeji.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://klt.hnxiangtu.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xwe.snrcjt.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kzb.tianlin.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://ohd.ydjk.org.cn

[N04] 斐波那契数列
来源：http://eer.xuetiantiany.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ovn.bjfxy.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://log.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cof.zhongyouzk.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mwe.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://clr.xuetiantiany.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://cgt.hongshengwenyu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ypo.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kdg.sxryk.cn

[N05] 最大公约数
来源：http://dqw.yonumen.top

Py:   math.gcd(a, b)
来源：http://kdl.fengsongda.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://eax.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://obx.dianchejie.cn


<!-- 参考信息 -->