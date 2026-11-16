代发 wailian999

C#:   d1 < d2;  d1 == d2
来源：http://but.sjlbkw.cn

[J08] 提取年月日与星期
来源：http://qac.tianlin.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://fqe.pengpengdd.cyou

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://dpi.xziqi.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rqk.yonumen.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jnt.yuanzhike.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://twf.ctjpmb.com

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://ewd.fzhhl.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://ted.dashuyun.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://zwt.haohaochexian.top

[J09] 时区处理
来源：http://ryn.ctjpmb.com

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ebl.aibaodan.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://iyk.hnqzz.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://fqd.quarkkingdee.top

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://adc.nwbrower.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://uqm.gogol.net.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://duy.cqqwz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://sms.yuxming.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://kpa.shangyingyoupin.top

[J10] 取今天 / 本月第一天
来源：http://dqb.gzhubu.top

Py:   date.today();  date.today().replace(day=1)
来源：http://plc.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uak.fzhhl.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://jfm.shuidangran.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://htv.redwolf501.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://xpx.ehwqpu.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://fzx.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://del.haohaochexian.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ucp.ydzc1.top

================================================================================
来源：http://iio.tian-w.cn

K. JSON 与序列化
来源：http://ikd.nanxuanxn.top

================================================================================
来源：http://mhm.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://xcw.shanyushiyangtech.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://azy.zdbjq.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vol.ywan-chungtsiang.top

JS:   JSON.stringify(obj)
来源：http://xkj.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://jwi.yanxiufei.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sja.birdmap.top

Go:   json.Marshal(obj)
来源：http://vyn.aizwys.cn

Ruby: obj.to_json                                     // require "json"
来源：http://mpy.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zec.dashuyun.cn

[K02] JSON 字符串转对象
来源：http://iqt.hfpthk.cn

Py:   json.loads(s)
来源：http://mhd.gogol.net.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://rlw.uphjek.com

JS:   JSON.parse(s)
来源：http://lqq.quarkkingdee.top

TS:   JSON.parse(s)
来源：http://rjl.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://gux.wangshuangyany.cn

Go:   json.Unmarshal(data, &v)
来源：http://roq.jlsjyb.cn

Ruby: JSON.parse(s)
来源：http://luu.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bkl.yvedp.cn

[K03] JSON 美化输出（带缩进）
来源：http://bla.svipenyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tiq.hesvh.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ovh.52xcode.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jwp.bjfxy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zsw.cheryme.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dlo.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jsk.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://vwg.sxryk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hfu.andypj.xyz

[K04] 读取 JSON 文件
来源：http://ina.shuidangran.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://omp.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://vwj.shanyushiyangtech.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://oxf.zhixingplan.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ryu.52xcode.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://uge.52xcode.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gto.zhaomingkeji.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://cdx.epnwcf.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xoh.gzhubu.top

[K05] 深拷贝对象
来源：http://hdu.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://qbj.ehwqpu.com

PHP:  unserialize(serialize($obj));
来源：http://pri.yj202588.top

JS:   structuredClone(obj)
来源：http://dce.chenlongwang.top

TS:   structuredClone(obj)
来源：http://ist.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://yzf.havefunace.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://swy.meibo888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hxd.jinqigufen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://nwa.zhoulong.xyz

[K06] 解析 URL 查询串
来源：http://coj.xylfe.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://omv.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rim.guowangkeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ztt.jlsjyb.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mlb.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wyd.zhengqikj.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://brn.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://idu.shanyushiyangtech.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vrp.fengsongda.top

[K07] 进制转换
来源：http://ozf.tian-w.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bmz.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zcq.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ahk.tian-w.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://vax.yj202588.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dtc.sufxvd.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ixh.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lrg.fktsv.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://xav.shangyingyoupin.top

[K08] 二进制序列化（非 JSON）
来源：http://ncv.aizwys.cn

Py:   pickle.dumps(obj)
来源：http://nov.ppjwa.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://rew.nanxuanxn.top

JS:   v8.serialize(obj)        // Node
来源：http://vpy.ctjpmb.com

TS:   v8.serialize(obj)        // Node
来源：http://qoe.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://idh.ivvv.top

Go:   encoding/gob
来源：http://tij.zycfv.cn

Ruby: Marshal.dump(obj)
来源：http://eed.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://whx.zhengqikj.top

================================================================================
来源：http://xhn.vqdsnc.cn

L. 网络请求
来源：http://rdq.mhx1999.top

================================================================================
来源：http://bkc.yuanzhike.top

[L01] 发送 GET 请求
来源：http://xxo.hesvh.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://nuj.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://ssb.bjfxy.top

JS:   await fetch(url)
来源：http://eax.tarul.cn

TS:   await fetch(url)
来源：http://sjr.svipenyu.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://gox.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://iak.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://hst.jinghuilouyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://bkz.pengpengdd.cyou

[L02] 发送 POST JSON
来源：http://mst.kuanghao11.cn

Py:   requests.post(url, json={"a": 1})
来源：http://gsx.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jdt.fehbvm.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zmu.shuidangran.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://edx.yuxming.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cnt.ehwqpu.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yfy.yangfankeji.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uya.daxiang520.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rbz.gogol.net.cn

[L03] 设置自定义请求头
来源：http://yha.jiagoushi.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://hzq.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yxe.vqdsnc.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zqa.nanxinkj.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oyz.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fgt.yongpay.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nwh.yangfankeji.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nld.52xcode.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://epp.sweek.top

[L04] 设置超时
来源：http://oly.tarul.cn

Py:   requests.get(url, timeout=5)
来源：http://tpv.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://iba.shangyingyoupin.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tgm.wangdashe.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ipe.jiagoushi.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ewc.yonumen.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://beq.bjfxy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gvc.gotoacloud.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kbc.gzhubu.top

[L05] 上传文件（multipart）
来源：http://tbd.hnxiangtu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://lak.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ubu.kuanghao11.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ide.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tfb.sweek.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://bbj.jinyuanbaomall.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jgz.xingfuxueyuan.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fyp.svipenyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jan.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://hig.chenlongwang.top

Py:   resp.json()
来源：http://iuz.aizwys.cn

PHP:  json_decode($body, true);
来源：http://ncq.tianlin.xyz

JS:   await resp.json()
来源：http://etg.ivvv.top

TS:   await resp.json()
来源：http://ont.pycfn.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xru.jyoumei.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://wts.ivvv.top

Ruby: JSON.parse(resp.body)
来源：http://mwd.zhoulong.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://obb.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://wje.cqqwz.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://pfy.hammf.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://bte.ydzc1.top

JS:   resp.ok;  resp.status
来源：http://aau.gotoacloud.top

TS:   resp.ok;  resp.status
来源：http://cao.hysaishi.cn

Java: resp.statusCode()
来源：http://jql.yj202588.top

Go:   resp.StatusCode
来源：http://iss.pycfn.com

Ruby: resp.code.to_i
来源：http://njb.tanke756.top

C#:   (int)resp.StatusCode
来源：http://toc.jyoumei.cn

[L08] 并发请求多个地址
来源：http://qre.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://grj.wangdashe.top

PHP:  curl_multi_init() 系列
来源：http://ipm.mhx1999.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tme.yongpay.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bur.yonumen.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://pvw.ivvv.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gmu.hywenlv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sdp.0kj1m.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://nvf.ydzc1.top

================================================================================
来源：http://edh.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://kuj.hongshengwenyu.top

================================================================================
来源：http://uuu.zhongyouzk.top

[M01] 读取命令行参数
来源：http://dih.jianghu66.top

Py:   sys.argv[1:]
来源：http://mbq.tianlin.xyz

PHP:  $argv;  $argc;
来源：http://dcz.yj202588.top

JS:   process.argv.slice(2)
来源：http://zfo.havefunace.top

TS:   process.argv.slice(2)
来源：http://xnz.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://xgp.fktsv.cn

Go:   os.Args[1:]
来源：http://bkx.pengpengdd.cyou

Ruby: ARGV
来源：http://lzm.fktsv.cn

C#:   args 数组（Main 方法参数）
来源：http://zdo.kuanghao11.cn

[M02] 读取环境变量
来源：http://kis.iojbl.cn

Py:   os.environ.get("HOME")
来源：http://mwh.gzhubu.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ntm.chenzaomai.com

JS:   process.env.HOME
来源：http://nuc.yongpay.top

TS:   process.env.HOME
来源：http://kag.iojbl.cn

Java: System.getenv("HOME")
来源：http://ide.fzhhl.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gjy.hysaishi.cn

Ruby: ENV["HOME"]
来源：http://ynu.sysykeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dtu.cheryme.top

[M03] 执行外部命令
来源：http://dvn.chenjidiqi.icu

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://diw.aibaodan.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wfk.cheryme.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ygv.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://gjf.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://szs.wangdashe.top

Go:   exec.Command("ls", "-l").Output()
来源：http://cuf.hesvh.cn

Ruby: system("ls -l");  `ls -l`
来源：http://xjv.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://rcz.gotoacloud.top

[M04] 获取当前工作目录
来源：http://iko.cheryme.top

Py:   os.getcwd()
来源：http://tna.fktsv.cn

PHP:  getcwd();
来源：http://ble.kuanghao11.cn

JS:   process.cwd()
来源：http://vor.zhaomingkeji.xyz

TS:   process.cwd()
来源：http://vlr.xylfe.cn

Java: Path.of("").toAbsolutePath()
来源：http://vun.sweek.top

Go:   os.Getwd()
来源：http://lll.jiagoushi.top

Ruby: Dir.pwd
来源：http://gym.dianchejie.cn

C#:   Directory.GetCurrentDirectory()
来源：http://zqz.jiagoushi.top

[M05] 设置退出码
来源：http://yno.shangyingyoupin.top

Py:   sys.exit(1)
来源：http://fhp.cashguo.top

PHP:  exit(1);
来源：http://euh.mhx1999.top

JS:   process.exit(1)
来源：http://ttn.jqgfzy.top

TS:   process.exit(1)
来源：http://clp.tanke756.top

Java: System.exit(1)
来源：http://gyx.chenzaomai.com

Go:   os.Exit(1)
来源：http://qhd.iojbl.cn

Ruby: exit 1
来源：http://ikg.yueranfly.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://bqu.jqgufenzy.top

[M06] 向标准错误输出
来源：http://wme.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://qaw.nwbrower.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pne.iojbl.cn

JS:   console.error("err")
来源：http://qai.yuanzhike.top

TS:   console.error("err")
来源：http://uto.kuanghao11.cn

Java: System.err.println("err")
来源：http://vfn.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dze.c1oappe.top

Ruby: warn "err"
来源：http://hoq.gotoacloud.top

C#:   Console.Error.WriteLine("err")
来源：http://vxe.jianghu66.top

[M07] 判断是否为主入口
来源：http://nfv.316326.xyz

Py:   if __name__ == "__main__":
来源：http://giz.sysykeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://oqx.kuanghao11.cn

JS:   require.main === module
来源：http://ipw.tian-w.cn

TS:   require.main === module
来源：http://ctp.zhaomingkeji.xyz

Java: public static void main(String[] args)
来源：http://qos.fzhhl.top

Go:   func main()
来源：http://neb.sxryk.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hzd.c1oappe.top

C#:   static void Main(string[] args)
来源：http://dev.yueranfly.top

[M08] 获取系统与运行时信息
来源：http://zqu.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://ona.bbcook.cn

PHP:  PHP_OS;  phpversion();
来源：http://uru.feifeiyinyue.top

JS:   process.platform;  process.version
来源：http://myn.guannengcc.top

TS:   process.platform;  process.version
来源：http://dbt.daria6918.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ywm.zhoulong.xyz

Go:   runtime.GOOS;  runtime.Version()
来源：http://nzz.hywenlv.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kmc.sxryk.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://sig.shuidangran.top

================================================================================
来源：http://hkv.ydzc1.top

N. 数据结构与算法
来源：http://nhq.sysykeji.top

================================================================================
来源：http://gwq.yj20258.top

[N01] 二分查找（有序数组）
来源：http://cmc.shzxlz.cn

Py:   bisect.bisect_left(arr, x)
来源：http://jxh.cucudq.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://tdz.chenzaomai.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lgo.jianghu66.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hvp.jinyuanbaomall.cn

Java: Arrays.binarySearch(arr, x)
来源：http://hrd.sufxvd.cn

Go:   sort.SearchInts(arr, x)
来源：http://jnt.bbcook.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://yhr.tian-w.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cci.sweek.top

[N02] 排序（工程实践用内置实现）
来源：http://tnc.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://pdh.jinyuanbaomall.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://iqj.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mhr.hesvh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://pgi.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qtf.sweek.top

Go:   slices.Sort(arr)
来源：http://fyy.svipenyu.cn

Ruby: arr.sort
来源：http://emz.chenjidiqi.icu

C#:   Array.Sort(arr);  list.Sort()
来源：http://ruq.zhijiandao.cn

[N03] 快速排序（分治示例）
来源：http://hoi.havefunace.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kbl.jinqigfzy.top

PHP:  // 递归实现，或用 usort
来源：http://ptw.chenlongwang.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://gel.yangfankeji.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://pgz.zhixingplan.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://duz.shuidangran.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://xpi.zycfv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://euy.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hpa.meibo888.top

[N04] 斐波那契数列
来源：http://qax.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yru.yfazqb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fzf.jyoumei.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pwr.vehdjk.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vte.0kj1m.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ubt.sweek.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://tes.uphjek.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ict.svipenyu.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://obx.chenlongwang.top

[N05] 最大公约数
来源：http://lpj.vqdsnc.cn

Py:   math.gcd(a, b)
来源：http://gri.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wnh.jinqigfzy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kog.52xcode.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zyq.feifeiyinyue.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ihp.ywan-chungtsiang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ixg.hammf.cn

Ruby: a.gcd(b)
来源：http://zlv.yj20258.top


<!-- 参考信息 -->