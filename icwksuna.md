代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://guh.wangshuangyany.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://tih.xziqi.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://bie.fktsv.cn

Ruby: d1 < d2;  d1 == d2
来源：http://pxj.tanke756.top

C#:   d1 < d2;  d1 == d2
来源：http://zrg.pengpengdd.cyou

[J08] 提取年月日与星期
来源：http://fgv.gotoacloud.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mwk.zdqjudy.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://wmn.uphjek.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://iny.jyoumei.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://pkd.zhiwuduotai.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dgu.hesvh.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://xdp.zycfv.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fvz.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://hpd.chenlongwang.top

[J09] 时区处理
来源：http://way.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://hju.zycfv.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://doh.hongshengwenyu.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://wmg.ydzc1.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://yat.pengpengdd.cyou

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ffp.0kj1m.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://nft.ppjwa.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://cfw.pengpengdd.cyou

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jgy.svipenyu.cn

[J10] 取今天 / 本月第一天
来源：http://yia.aizwys.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ecw.yj20258888.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://lok.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hse.yueranfly.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://poq.shanyushiyangtech.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ioi.zdqjudy.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://adp.hysaishi.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://txf.yvedp.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xag.jqgfzy.top

================================================================================
来源：http://bgu.xylfe.cn

K. JSON 与序列化
来源：http://bdk.guowangkeji.top

================================================================================
来源：http://udq.havefunace.top

[K01] 对象转 JSON 字符串
来源：http://bry.zycfv.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://awy.52xcode.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://cgr.daxiang520.top

JS:   JSON.stringify(obj)
来源：http://mfm.uphjek.com

TS:   JSON.stringify(obj)
来源：http://mph.feifeiyinyue.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://max.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://lrg.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://ybg.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://kdu.chenzaomai.com

[K02] JSON 字符串转对象
来源：http://oee.zycfv.cn

Py:   json.loads(s)
来源：http://foa.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kcr.fzhhl.top

JS:   JSON.parse(s)
来源：http://gjz.zhoulong.xyz

TS:   JSON.parse(s)
来源：http://zuc.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wox.jqgfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://fls.wangshuangyany.cn

Ruby: JSON.parse(s)
来源：http://rko.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://tia.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://hav.xylfe.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://why.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://oqq.yj20258888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://wof.yj202588.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zxw.zhixingplan.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://oyf.jiagoushi.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://sgy.316326.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://udz.hcnkem.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jin.yj20258888.top

[K04] 读取 JSON 文件
来源：http://spq.yonumen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lht.ybcxt.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ogz.jinqigfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://any.hfpthk.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mcm.zhiwuduotai.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://phh.nwbrower.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://icq.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://wzb.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bhl.yonumen.top

[K05] 深拷贝对象
来源：http://qws.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://wvf.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://cst.yj202588.top

JS:   structuredClone(obj)
来源：http://fta.hnqzz.top

TS:   structuredClone(obj)
来源：http://kzj.jqgufenzy.top

Java: // 手写拷贝构造，或序列化往返
来源：http://qfk.sweek.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lyo.xuanzx.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://klf.hywenlv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://aao.sufxvd.cn

[K06] 解析 URL 查询串
来源：http://uoj.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dmb.guannengcc.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lxj.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://urn.fktsv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vuh.yj20258.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dug.feifeiyinyue.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://zru.shangyingyoupin.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fhd.jinqigufen.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yyf.xylfe.cn

[K07] 进制转换
来源：http://lvq.shanyushiyangkeji.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cxt.smart0.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wdb.nwbrower.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qvd.jinqigufen.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://jiu.pycfn.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pzd.aibaodan.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wfz.yanxiufei.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vnh.zycfv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vzx.gotoacloud.top

[K08] 二进制序列化（非 JSON）
来源：http://hbe.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://snr.hongshengwenyu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yhl.shangyingyoupin.top

JS:   v8.serialize(obj)        // Node
来源：http://qvr.gotoacloud.top

TS:   v8.serialize(obj)        // Node
来源：http://tig.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://vxx.ctjpmb.com

Go:   encoding/gob
来源：http://cba.shangyingyoupin.top

Ruby: Marshal.dump(obj)
来源：http://awl.smart0.xyz

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ghb.zhixingplan.top

================================================================================
来源：http://eye.uphjek.com

L. 网络请求
来源：http://qwu.gzhubu.top

================================================================================
来源：http://lfc.tian-w.cn

[L01] 发送 GET 请求
来源：http://lsq.daria6918.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://gal.epnwcf.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ztz.jiagoushi.top

JS:   await fetch(url)
来源：http://pyq.nanxuanxn.top

TS:   await fetch(url)
来源：http://doh.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ehr.jinyuanbaomall.cn

Go:   resp, err := http.Get(url)
来源：http://xto.sysykeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://cdu.sjlbkw.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://lmi.tianlin.xyz

[L02] 发送 POST JSON
来源：http://pue.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://mit.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wjj.jyoumei.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oyw.zdqjudy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dxz.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vab.wangdashe.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dxm.fehbvm.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ucb.bbcook.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://btg.9152youxi.cn

[L03] 设置自定义请求头
来源：http://ulv.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://eou.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://oyw.fktsv.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bxb.jyoumei.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vlo.haohaochexian.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qrn.yvedp.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://cjr.yueranfly.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://jje.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jml.wangdashe.top

[L04] 设置超时
来源：http://dui.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://rby.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dmj.bjfxy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eoe.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gzg.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://dys.xinyue.icu

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vjq.fanxiaobao.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tmr.chenjidiqi.icu

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://hjy.pengpengdd.cyou

[L05] 上传文件（multipart）
来源：http://dde.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bih.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://wiy.guowangkeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://fde.bjfxy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vid.gzhubu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kja.cheryme.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://hoq.ydjk.org.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mmd.birdmap.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://vey.ivvv.top

[L06] 解析响应为 JSON
来源：http://ljs.jinyuanbaomall.cn

Py:   resp.json()
来源：http://sqq.chenjidiqi.icu

PHP:  json_decode($body, true);
来源：http://csx.jianghu66.top

JS:   await resp.json()
来源：http://rea.fehbvm.com

TS:   await resp.json()
来源：http://xrn.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://tzo.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uid.shanyushiyangkeji.top

Ruby: JSON.parse(resp.body)
来源：http://fgq.hcnkem.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dqm.vqdsnc.cn

[L07] 处理 HTTP 状态码
来源：http://cay.gaohongyu789.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://epk.quarkkingdee.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jok.vehdjk.com

JS:   resp.ok;  resp.status
来源：http://gwd.kuanghao11.cn

TS:   resp.ok;  resp.status
来源：http://tts.316326.xyz

Java: resp.statusCode()
来源：http://oft.chenzaomai.com

Go:   resp.StatusCode
来源：http://kic.yongpay.top

Ruby: resp.code.to_i
来源：http://gll.jqgfzy.top

C#:   (int)resp.StatusCode
来源：http://oxy.zhongyouzk.top

[L08] 并发请求多个地址
来源：http://bmo.zdbjq.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://krp.hfpthk.cn

PHP:  curl_multi_init() 系列
来源：http://ozn.pengpengdd.cyou

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ldd.havefunace.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hya.pengpengdd.cyou

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://nbe.316326.xyz

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iki.cashguo.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://uat.zhaomingkeji.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cvn.vqdsnc.cn

================================================================================
来源：http://psi.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://wpe.shanyushiyangtech.top

================================================================================
来源：http://kse.pengpengdd.cyou

[M01] 读取命令行参数
来源：http://nyd.cashguo.top

Py:   sys.argv[1:]
来源：http://zdx.daxiang520.top

PHP:  $argv;  $argc;
来源：http://dnf.hcnkem.com

JS:   process.argv.slice(2)
来源：http://jws.316326.xyz

TS:   process.argv.slice(2)
来源：http://gao.pengpengdd.cyou

Java: args 数组（main 方法参数）
来源：http://eqa.daxiang520.top

Go:   os.Args[1:]
来源：http://xbd.vehdjk.com

Ruby: ARGV
来源：http://eor.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://yev.ctjpmb.com

[M02] 读取环境变量
来源：http://wcy.jianghu66.top

Py:   os.environ.get("HOME")
来源：http://gox.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tac.chenzaomai.com

JS:   process.env.HOME
来源：http://lxw.zhengqikj.top

TS:   process.env.HOME
来源：http://fqq.gotoacloud.top

Java: System.getenv("HOME")
来源：http://xgc.guowangkeji.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://zyh.cheryme.top

Ruby: ENV["HOME"]
来源：http://fhx.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://znq.sxryk.cn

[M03] 执行外部命令
来源：http://ecq.yj20258.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dbr.yj20258888.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jmy.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://nec.guannengcc.top

TS:   child_process.execSync("ls -l").toString()
来源：http://eaa.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://edp.epnwcf.com

Go:   exec.Command("ls", "-l").Output()
来源：http://vxt.vqdsnc.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dqx.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://ttu.dashuyun.cn

[M04] 获取当前工作目录
来源：http://ttp.316326.xyz

Py:   os.getcwd()
来源：http://sda.yj20258.top

PHP:  getcwd();
来源：http://lrr.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://hwd.feifeiyinyue.top

TS:   process.cwd()
来源：http://vuu.bbcook.cn

Java: Path.of("").toAbsolutePath()
来源：http://vau.cqqwz.cn

Go:   os.Getwd()
来源：http://wli.sweek.top

Ruby: Dir.pwd
来源：http://psm.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://xfi.hysaishi.cn

[M05] 设置退出码
来源：http://nkg.zdbjq.cn

Py:   sys.exit(1)
来源：http://gew.jinqigufen.top

PHP:  exit(1);
来源：http://tvt.zhoulong.xyz

JS:   process.exit(1)
来源：http://knx.jqgfzy.top

TS:   process.exit(1)
来源：http://cta.tanke756.top

Java: System.exit(1)
来源：http://joi.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://gkn.wangshuangyany.cn

Ruby: exit 1
来源：http://hpk.xylfe.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://fhz.zdqjudy.top

[M06] 向标准错误输出
来源：http://apv.jinqigfzy.top

Py:   print("err", file=sys.stderr)
来源：http://fzo.sysykeji.top

PHP:  fwrite(STDERR, "err\n");
来源：http://imp.tianlin.xyz

JS:   console.error("err")
来源：http://mno.gzhubu.top

TS:   console.error("err")
来源：http://eaj.chenjidiqi.icu

Java: System.err.println("err")
来源：http://dwu.ppjwa.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dew.9152youxi.cn

Ruby: warn "err"
来源：http://mci.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://mrl.nwbrower.top

[M07] 判断是否为主入口
来源：http://pvc.pengpengdd.cyou

Py:   if __name__ == "__main__":
来源：http://ybk.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bvc.ydzc1.top

JS:   require.main === module
来源：http://oxo.daxiang520.top

TS:   require.main === module
来源：http://wlf.uphjek.com

Java: public static void main(String[] args)
来源：http://ndc.yj20258888.top

Go:   func main()
来源：http://tvs.fzhhl.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://geo.birdmap.top

C#:   static void Main(string[] args)
来源：http://utw.fzhhl.top

[M08] 获取系统与运行时信息
来源：http://dee.aizwys.cn

Py:   platform.system();  platform.python_version()
来源：http://nxz.316326.xyz

PHP:  PHP_OS;  phpversion();
来源：http://fur.daria6918.cn

JS:   process.platform;  process.version
来源：http://slh.meibo888.top

TS:   process.platform;  process.version
来源：http://khe.shanyushiyangtech.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xgb.bbcook.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://btd.sxryk.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://zif.jinghuilouyu.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://tvk.yuxming.cn

================================================================================
来源：http://xbq.tian-w.cn

N. 数据结构与算法
来源：http://drp.zdbjq.cn

================================================================================
来源：http://tfh.hammf.cn

[N01] 二分查找（有序数组）
来源：http://lfn.snrcjt.cn

Py:   bisect.bisect_left(arr, x)
来源：http://kbp.tarul.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://hlx.zhixingplan.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://mug.yfazqb.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://cvj.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://dts.wangdashe.top

Go:   sort.SearchInts(arr, x)
来源：http://vfg.aizwys.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yyp.uphjek.com

C#:   Array.BinarySearch(arr, x)
来源：http://jas.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://gkb.yangfankeji.com

Py:   sorted(arr);  arr.sort()
来源：http://igf.fzhhl.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gxo.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://ofi.fanxiaobao.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://vva.jiagoushi.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ijd.kuanghao11.cn

Go:   slices.Sort(arr)
来源：http://tye.yonumen.top

Ruby: arr.sort
来源：http://edp.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qvt.hnqzz.top

[N03] 快速排序（分治示例）
来源：http://fuy.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://dww.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://jht.kuanghao11.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://koq.jinqigfzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://igt.hcnkem.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://gbj.ydjk.org.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wpg.zhoulong.xyz

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ral.nanxinkj.top

C#:   // 手写递归，或 Array.Sort
来源：http://mjd.gzhubu.top

[N04] 斐波那契数列
来源：http://evi.chenjidiqi.icu

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://but.nanxinkj.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://vkm.yvedp.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mji.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://aka.zhixingplan.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mud.birdmap.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ugv.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://kfn.yfazqb.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lny.wangdashe.top

[N05] 最大公约数
来源：http://iks.quarkkingdee.top

Py:   math.gcd(a, b)
来源：http://jpw.chenlongwang.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://cuv.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bqh.316326.xyz


<!-- 参考信息 -->