代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://rwv.zdbjq.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://zjl.xylfe.cn

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://eur.nwbrower.top

Ruby: d1 < d2;  d1 == d2
来源：http://eqa.smart0.xyz

C#:   d1 < d2;  d1 == d2
来源：http://dxn.c1oappe.top

[J08] 提取年月日与星期
来源：http://fib.birdmap.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://mkk.0kj1m.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://zel.cashguo.top

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://tvo.tian-w.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://quf.zhijiandao.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://dpf.shuidangran.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fkq.bbcook.cn

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://tgt.yj20258888.top

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://mth.cqqwz.cn

[J09] 时区处理
来源：http://soz.bjfxy.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://gtw.jinqigufen.top

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://fkl.fanxiaobao.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://mie.sufxvd.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://sfs.pycfn.com

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ocq.dianchejie.cn

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://pzd.xingfuxueyuan.xyz

Ruby: Time.now.getlocal("+08:00")
来源：http://sna.chenzaomai.com

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://ngl.iojbl.cn

[J10] 取今天 / 本月第一天
来源：http://zmm.tarul.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ddf.hesvh.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://zbx.jianghu66.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zmx.pycfn.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://gyc.zdqjudy.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://svp.zhiwuduotai.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://frh.sweek.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mbp.jinghuilouyu.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wey.tian-w.cn

================================================================================
来源：http://ksn.smart0.xyz

K. JSON 与序列化
来源：http://nit.chenlongwang.top

================================================================================
来源：http://rma.xuanzx.com

[K01] 对象转 JSON 字符串
来源：http://pwt.guannengcc.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://pzt.yj202588.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kiz.pycfn.com

JS:   JSON.stringify(obj)
来源：http://pso.ybcxt.top

TS:   JSON.stringify(obj)
来源：http://ixt.zhongyouzk.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://sln.ywan-chungtsiang.top

Go:   json.Marshal(obj)
来源：http://bdm.hesvh.cn

Ruby: obj.to_json                                     // require "json"
来源：http://jss.xuetiantiany.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://sfk.daria6918.cn

[K02] JSON 字符串转对象
来源：http://vkg.iojbl.cn

Py:   json.loads(s)
来源：http://kvz.yueranfly.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://fkf.cheryme.top

JS:   JSON.parse(s)
来源：http://bmd.haohaochexian.top

TS:   JSON.parse(s)
来源：http://its.wangdashe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rmb.svipenyu.cn

Go:   json.Unmarshal(data, &v)
来源：http://gpw.jiagoushi.top

Ruby: JSON.parse(s)
来源：http://sbo.chenzaomai.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dpu.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://kll.ivvv.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://wom.sufxvd.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lpg.iojbl.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://lok.jiagoushi.top

TS:   JSON.stringify(obj, null, 2)
来源：http://syy.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://kzw.hywenlv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fwz.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://slp.hfpthk.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://pqe.shuidangran.top

[K04] 读取 JSON 文件
来源：http://xxz.jinqigfzy.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kuq.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://udu.52xcode.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rcq.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://wuc.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ybk.cdnleiting.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mfr.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://rvz.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://exh.c1oappe.top

[K05] 深拷贝对象
来源：http://pee.chenlongwang.top

Py:   copy.deepcopy(obj)
来源：http://koo.ppjwa.cn

PHP:  unserialize(serialize($obj));
来源：http://lyf.jinyuanbaomall.cn

JS:   structuredClone(obj)
来源：http://tpg.hfpthk.cn

TS:   structuredClone(obj)
来源：http://wmv.zhoulong.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://wml.yonumen.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wyc.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kqg.aibaodan.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://qbb.guowangkeji.top

[K06] 解析 URL 查询串
来源：http://gtp.hongshengwenyu.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://pjy.cashguo.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rmc.ydjk.org.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pth.jqgfzy.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jrq.pengpengdd.cyou

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vav.birdmap.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://jao.zdqjudy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cdn.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://aat.xinyue.icu

[K07] 进制转换
来源：http://gmn.jinqigfzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://tnf.xingfuxueyuan.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hdw.yueranfly.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://pun.316326.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://lqf.zdbjq.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://gak.nwbrower.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rzv.jinqigufen.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://bbq.shanyushiyangtech.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uio.9152youxi.cn

[K08] 二进制序列化（非 JSON）
来源：http://lku.sweek.top

Py:   pickle.dumps(obj)
来源：http://ngf.uphjek.com

PHP:  serialize($obj);  unserialize($s);
来源：http://ctk.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://wci.fktsv.cn

TS:   v8.serialize(obj)        // Node
来源：http://ngi.cqqwz.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eia.gogol.net.cn

Go:   encoding/gob
来源：http://xfo.tianlin.xyz

Ruby: Marshal.dump(obj)
来源：http://hgd.wangdashe.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dbi.cdnleiting.top

================================================================================
来源：http://kyu.epnwcf.com

L. 网络请求
来源：http://zzn.jinghuilouyu.cn

================================================================================
来源：http://axg.pengpengdd.cyou

[L01] 发送 GET 请求
来源：http://hkr.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://oew.smart0.xyz

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://otz.andypj.xyz

JS:   await fetch(url)
来源：http://ytq.yfazqb.com

TS:   await fetch(url)
来源：http://qto.hnxiangtu.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vyy.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://hss.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ffv.zhongyouzk.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mep.xinyue.icu

[L02] 发送 POST JSON
来源：http://mxj.52xcode.cn

Py:   requests.post(url, json={"a": 1})
来源：http://wlq.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uvq.vqdsnc.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ujo.tian-w.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fns.52xcode.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vhq.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ksz.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://tsr.xuanzx.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://uuj.ppjwa.cn

[L03] 设置自定义请求头
来源：http://jzz.tanke756.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://moe.ppjwa.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://omr.fehbvm.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://kxh.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blq.chenzaomai.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://jxg.9152youxi.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yvx.xziqi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nhf.uphjek.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mlq.daria6918.cn

[L04] 设置超时
来源：http://uwh.wangdashe.top

Py:   requests.get(url, timeout=5)
来源：http://kko.hesvh.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://oxj.52xcode.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eku.ybcxt.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://olh.zhiwuduotai.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://pur.yj20258.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nfn.dianchejie.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yqd.cucudq.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://kkg.havefunace.top

[L05] 上传文件（multipart）
来源：http://ikf.feifeiyinyue.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://mpu.zhaomingkeji.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://bds.tian-w.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://sfk.dianchejie.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mps.yanxiufei.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dqq.hysaishi.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://qns.hesvh.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://hcm.wangdashe.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://cwe.shanyushiyangtech.top

[L06] 解析响应为 JSON
来源：http://fdw.yj20258888.top

Py:   resp.json()
来源：http://eok.c1oappe.top

PHP:  json_decode($body, true);
来源：http://ins.tarul.cn

JS:   await resp.json()
来源：http://wrf.fanxiaobao.xyz

TS:   await resp.json()
来源：http://cls.iojbl.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jdi.fehbvm.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jaz.hesvh.cn

Ruby: JSON.parse(resp.body)
来源：http://ksg.hnxiangtu.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rkl.quarkkingdee.top

[L07] 处理 HTTP 状态码
来源：http://gaq.fanxiaobao.xyz

Py:   resp.status_code;  resp.raise_for_status()
来源：http://htz.ehwqpu.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://rjr.daria6918.cn

JS:   resp.ok;  resp.status
来源：http://ncq.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://vfw.hfpthk.cn

Java: resp.statusCode()
来源：http://fpt.dianchejie.cn

Go:   resp.StatusCode
来源：http://gbi.fktsv.cn

Ruby: resp.code.to_i
来源：http://svh.fktsv.cn

C#:   (int)resp.StatusCode
来源：http://mkr.bjfxy.top

[L08] 并发请求多个地址
来源：http://ctd.yj20258.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://bor.shzxlz.cn

PHP:  curl_multi_init() 系列
来源：http://ilv.wangshuangyany.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zhg.tian-w.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dok.cdnleiting.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uql.hcnkem.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qtd.sjlbkw.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://mun.bjfxy.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qcp.tian-w.cn

================================================================================
来源：http://knh.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://zob.ydjk.org.cn

================================================================================
来源：http://vwn.cdnleiting.top

[M01] 读取命令行参数
来源：http://ioe.xuetiantiany.cn

Py:   sys.argv[1:]
来源：http://ewx.xingfuxueyuan.xyz

PHP:  $argv;  $argc;
来源：http://avz.fanxiaobao.xyz

JS:   process.argv.slice(2)
来源：http://ksn.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://qpp.yuanzhike.top

Java: args 数组（main 方法参数）
来源：http://yti.iojbl.cn

Go:   os.Args[1:]
来源：http://syz.kuanghao11.cn

Ruby: ARGV
来源：http://rup.wangshuangyany.cn

C#:   args 数组（Main 方法参数）
来源：http://gaz.shuidangran.top

[M02] 读取环境变量
来源：http://ybs.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://xwf.hywenlv.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://naw.havefunace.top

JS:   process.env.HOME
来源：http://xnd.jiagoushi.top

TS:   process.env.HOME
来源：http://che.feifeiyinyue.top

Java: System.getenv("HOME")
来源：http://efe.chenlongwang.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://yxp.yj20258.top

Ruby: ENV["HOME"]
来源：http://loi.zhaomingkeji.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jnl.jinyuanbaomall.cn

[M03] 执行外部命令
来源：http://kmn.bjfxy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mus.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://chg.hysaishi.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://hvr.uphjek.com

TS:   child_process.execSync("ls -l").toString()
来源：http://yuf.zdqjudy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://yqf.gogol.net.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wpt.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://lpx.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://mnk.yanxiufei.cn

[M04] 获取当前工作目录
来源：http://cdm.pengpengdd.cyou

Py:   os.getcwd()
来源：http://uiy.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://rdi.hysaishi.cn

JS:   process.cwd()
来源：http://ugr.sweek.top

TS:   process.cwd()
来源：http://ied.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://trt.gaohongyu789.top

Go:   os.Getwd()
来源：http://wqi.gzhubu.top

Ruby: Dir.pwd
来源：http://oyb.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://ffz.yongpay.top

[M05] 设置退出码
来源：http://hzc.hnxiangtu.top

Py:   sys.exit(1)
来源：http://ryb.sjlbkw.cn

PHP:  exit(1);
来源：http://ahn.jinghuilouyu.cn

JS:   process.exit(1)
来源：http://nov.uphjek.com

TS:   process.exit(1)
来源：http://aat.iojbl.cn

Java: System.exit(1)
来源：http://npq.zhijiandao.cn

Go:   os.Exit(1)
来源：http://wyv.jinqigufen.top

Ruby: exit 1
来源：http://poc.ywan-chungtsiang.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uic.zhengqikj.top

[M06] 向标准错误输出
来源：http://mct.nanxuanxn.top

Py:   print("err", file=sys.stderr)
来源：http://tfn.hcnkem.com

PHP:  fwrite(STDERR, "err\n");
来源：http://vvl.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://ogi.havefunace.top

TS:   console.error("err")
来源：http://opj.sysykeji.top

Java: System.err.println("err")
来源：http://tdo.shanyushiyangkeji.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bhz.iojbl.cn

Ruby: warn "err"
来源：http://oeu.yj20258888.top

C#:   Console.Error.WriteLine("err")
来源：http://hvi.pycfn.com

[M07] 判断是否为主入口
来源：http://fgz.sjlbkw.cn

Py:   if __name__ == "__main__":
来源：http://sey.hongshengwenyu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://rwl.zhaomingkeji.xyz

JS:   require.main === module
来源：http://hsj.jinyuanbaomall.cn

TS:   require.main === module
来源：http://dph.yanxiufei.cn

Java: public static void main(String[] args)
来源：http://plj.mhx1999.top

Go:   func main()
来源：http://xma.hysaishi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mec.nanxinkj.top

C#:   static void Main(string[] args)
来源：http://lwp.yfazqb.com

[M08] 获取系统与运行时信息
来源：http://gif.daria6918.cn

Py:   platform.system();  platform.python_version()
来源：http://bvw.shanyushiyangtech.top

PHP:  PHP_OS;  phpversion();
来源：http://gts.fzhhl.top

JS:   process.platform;  process.version
来源：http://szf.yj20258888.top

TS:   process.platform;  process.version
来源：http://qia.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wlz.ivvv.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rhn.cucudq.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://srn.fktsv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://qdz.wangshuangyany.cn

================================================================================
来源：http://wvz.hammf.cn

N. 数据结构与算法
来源：http://mne.jqgfzy.top

================================================================================
来源：http://vyw.jinyuanbaomall.cn

[N01] 二分查找（有序数组）
来源：http://waz.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ads.xuanzx.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://gye.yfazqb.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://opv.xinyue.icu

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ehh.pengpengdd.cyou

Java: Arrays.binarySearch(arr, x)
来源：http://xle.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://bvj.jianghu66.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fjb.xziqi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://clh.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://iyo.haohaochexian.top

Py:   sorted(arr);  arr.sort()
来源：http://rpg.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oil.jiagoushi.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://oxy.xuetiantiany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://vhc.yfazqb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qjf.zdbjq.cn

Go:   slices.Sort(arr)
来源：http://cbr.daria6918.cn

Ruby: arr.sort
来源：http://hmx.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rxr.zhixingplan.top

[N03] 快速排序（分治示例）
来源：http://qzx.cheryme.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kck.yvedp.cn

PHP:  // 递归实现，或用 usort
来源：http://arl.havefunace.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://aww.jiagoushi.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sag.ivvv.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ktw.zhixingplan.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yio.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://tgb.gogol.net.cn

C#:   // 手写递归，或 Array.Sort
来源：http://eel.jyoumei.cn

[N04] 斐波那契数列
来源：http://egh.jlsjyb.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://vnf.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tha.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ffa.gzhubu.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://jjc.cdnleiting.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pyx.hongshengwenyu.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hwk.hcnkem.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://qvs.feifeiyinyue.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://szj.cheryme.top

[N05] 最大公约数
来源：http://dty.bbcook.cn

Py:   math.gcd(a, b)
来源：http://ovm.zhengqikj.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://alm.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ugy.zhijiandao.cn


<!-- 参考信息 -->