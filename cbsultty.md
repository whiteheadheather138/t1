代发 wailian999

TS:   d1.getTime() < d2.getTime()
来源：http://xhv.guannengcc.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://mrn.hnxiangtu.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ufy.52xcode.cn

Ruby: d1 < d2;  d1 == d2
来源：http://tcj.yongpay.top

C#:   d1 < d2;  d1 == d2
来源：http://blk.jinyuanbaomall.cn

[J08] 提取年月日与星期
来源：http://oau.smart0.xyz

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://lym.tarul.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ohd.xingfuxueyuan.xyz

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://egi.cucudq.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://jnd.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://ubi.sysykeji.top

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://itj.zhaomingkeji.xyz

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://eje.ehwqpu.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://sfh.chenlongwang.top

[J09] 时区处理
来源：http://mzb.jinqigufen.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://ooy.xylfe.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://bup.zhoulong.xyz

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://gsn.ydjk.org.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://kgu.chenlongwang.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://ebv.haohaochexian.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://qpy.haohaochexian.top

Ruby: Time.now.getlocal("+08:00")
来源：http://uft.gogol.net.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://xzf.wangshuangyany.cn

[J10] 取今天 / 本月第一天
来源：http://lae.wangshuangyany.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://ovf.jinqigfzy.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sbb.gotoacloud.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qlc.sxryk.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://wyz.52xcode.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qsm.pycfn.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aux.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://zww.gzhubu.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://skx.dashuyun.cn

================================================================================
来源：http://axv.yanxiufei.cn

K. JSON 与序列化
来源：http://ppv.xuetiantiany.cn

================================================================================
来源：http://tjw.cashguo.top

[K01] 对象转 JSON 字符串
来源：http://rhr.shanyushiyangkeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fpm.jyoumei.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xqu.tarul.cn

JS:   JSON.stringify(obj)
来源：http://afs.havefunace.top

TS:   JSON.stringify(obj)
来源：http://fij.jlsjyb.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cia.xylfe.cn

Go:   json.Marshal(obj)
来源：http://fbt.pengpengdd.cyou

Ruby: obj.to_json                                     // require "json"
来源：http://juh.shuidangran.top

C#:   JsonSerializer.Serialize(obj)
来源：http://eah.jianghu66.top

[K02] JSON 字符串转对象
来源：http://iii.tian-w.cn

Py:   json.loads(s)
来源：http://aov.jlsjyb.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://wnw.jinqigufen.top

JS:   JSON.parse(s)
来源：http://bol.fengsongda.top

TS:   JSON.parse(s)
来源：http://cwi.zhixingplan.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://nyo.hongshengwenyu.top

Go:   json.Unmarshal(data, &v)
来源：http://hnv.bbcook.cn

Ruby: JSON.parse(s)
来源：http://ojg.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zoc.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://yiq.jqgufenzy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cmv.shanyushiyangtech.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ihd.snrcjt.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jky.cucudq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ypw.guowangkeji.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ppo.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://spl.zhixingplan.top

Ruby: JSON.pretty_generate(obj)
来源：http://ipj.cashguo.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://aze.havefunace.top

[K04] 读取 JSON 文件
来源：http://mtr.tarul.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vts.tian-w.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ejr.aizwys.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pjg.ywan-chungtsiang.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dyl.hnqzz.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wgy.ppjwa.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yyu.ctjpmb.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://ysn.gzhubu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://qhz.zhongyouzk.top

[K05] 深拷贝对象
来源：http://txo.pengpengdd.cyou

Py:   copy.deepcopy(obj)
来源：http://xiy.hammf.cn

PHP:  unserialize(serialize($obj));
来源：http://hyr.aizwys.cn

JS:   structuredClone(obj)
来源：http://bgk.zhoulong.xyz

TS:   structuredClone(obj)
来源：http://jgk.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://duv.pengpengdd.cyou

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tde.zycfv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hrx.chenjidiqi.icu

C#:   // 序列化往返，或自定义 Clone
来源：http://lcn.yuxming.cn

[K06] 解析 URL 查询串
来源：http://ykt.wangdashe.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yjx.hammf.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://stw.0kj1m.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://byw.fehbvm.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ask.ctjpmb.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://dqy.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://kfh.smart0.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://aaj.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://njo.dianchejie.cn

[K07] 进制转换
来源：http://lsl.zycfv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://nnh.shangyingyoupin.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yaq.fehbvm.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://rqf.nwbrower.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://djh.haohaochexian.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://hnk.9152youxi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://tzc.zhixingplan.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hmk.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://agx.yvedp.cn

[K08] 二进制序列化（非 JSON）
来源：http://axy.shanyushiyangtech.top

Py:   pickle.dumps(obj)
来源：http://hsj.chenlongwang.top

PHP:  serialize($obj);  unserialize($s);
来源：http://olq.yvedp.cn

JS:   v8.serialize(obj)        // Node
来源：http://ulq.yuanzhike.top

TS:   v8.serialize(obj)        // Node
来源：http://upa.ivvv.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xmq.chenlongwang.top

Go:   encoding/gob
来源：http://jdu.jyoumei.cn

Ruby: Marshal.dump(obj)
来源：http://dbr.yanxiufei.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://byy.zdbjq.cn

================================================================================
来源：http://pmh.yj20258.top

L. 网络请求
来源：http://ezw.ydjk.org.cn

================================================================================
来源：http://blj.fehbvm.com

[L01] 发送 GET 请求
来源：http://nuq.kuanghao11.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uxa.zdqjudy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://xnb.sufxvd.cn

JS:   await fetch(url)
来源：http://ctb.fktsv.cn

TS:   await fetch(url)
来源：http://nyb.hnqzz.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vmj.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://ile.shzxlz.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://zdz.sxryk.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zyv.chenjidiqi.icu

[L02] 发送 POST JSON
来源：http://eul.chenzaomai.com

Py:   requests.post(url, json={"a": 1})
来源：http://hce.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uhg.yongpay.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://scs.aizwys.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dpr.tianlin.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://bmg.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aas.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://rqi.shzxlz.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qxo.xylfe.cn

[L03] 设置自定义请求头
来源：http://xga.52xcode.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ywx.wangshuangyany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ubi.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fbc.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oox.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xqa.yuanzhike.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uxe.daria6918.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://btc.zhengqikj.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fdm.sufxvd.cn

[L04] 设置超时
来源：http://kbd.gogol.net.cn

Py:   requests.get(url, timeout=5)
来源：http://srj.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://hvq.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ujo.svipenyu.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yee.chenlongwang.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://uty.andypj.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://noy.meibo888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ygq.sufxvd.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://gta.fengsongda.top

[L05] 上传文件（multipart）
来源：http://cen.aizwys.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://bpd.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://klv.fehbvm.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vep.0kj1m.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ilu.hysaishi.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://usi.zhijiandao.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nbe.sxryk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ngo.shzxlz.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lkt.jyoumei.cn

[L06] 解析响应为 JSON
来源：http://elr.xuanzx.com

Py:   resp.json()
来源：http://tqv.yueranfly.top

PHP:  json_decode($body, true);
来源：http://vhf.xinyue.icu

JS:   await resp.json()
来源：http://mon.cucudq.cn

TS:   await resp.json()
来源：http://msy.svipenyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://rts.daxiang520.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mlf.shuidangran.top

Ruby: JSON.parse(resp.body)
来源：http://kfu.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://whh.jinqigfzy.top

[L07] 处理 HTTP 状态码
来源：http://dwb.guowangkeji.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://prg.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qdf.aibaodan.cn

JS:   resp.ok;  resp.status
来源：http://gsr.svipenyu.cn

TS:   resp.ok;  resp.status
来源：http://bln.hcnkem.com

Java: resp.statusCode()
来源：http://vde.zdbjq.cn

Go:   resp.StatusCode
来源：http://vtl.xinyue.icu

Ruby: resp.code.to_i
来源：http://xnl.uphjek.com

C#:   (int)resp.StatusCode
来源：http://plc.yj20258.top

[L08] 并发请求多个地址
来源：http://rlm.hfpthk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://npt.zhongyouzk.top

PHP:  curl_multi_init() 系列
来源：http://hhm.hnqzz.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://xyi.nanxuanxn.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://awg.fehbvm.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ojq.jqgufenzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iqj.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jky.daria6918.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gbq.shangyingyoupin.top

================================================================================
来源：http://obj.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://azf.sweek.top

================================================================================
来源：http://yqm.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://duf.jinqigfzy.top

Py:   sys.argv[1:]
来源：http://fvi.zhoulong.xyz

PHP:  $argv;  $argc;
来源：http://jte.zhaomingkeji.xyz

JS:   process.argv.slice(2)
来源：http://vgj.chenjidiqi.icu

TS:   process.argv.slice(2)
来源：http://npr.hammf.cn

Java: args 数组（main 方法参数）
来源：http://vng.kuanghao11.cn

Go:   os.Args[1:]
来源：http://ggq.hcnkem.com

Ruby: ARGV
来源：http://nno.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://tvo.cqqwz.cn

[M02] 读取环境变量
来源：http://nwz.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://ghq.chenlongwang.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://zck.shangyingyoupin.top

JS:   process.env.HOME
来源：http://fpm.ppjwa.cn

TS:   process.env.HOME
来源：http://zey.zhoulong.xyz

Java: System.getenv("HOME")
来源：http://ldx.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://fuh.hcnkem.com

Ruby: ENV["HOME"]
来源：http://abd.hnqzz.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://phn.wangdashe.top

[M03] 执行外部命令
来源：http://gfy.dianchejie.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://tro.zdqjudy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ngz.shuidangran.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lgc.daxiang520.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ymz.xylfe.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://awl.shanyushiyangkeji.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mdw.xylfe.cn

Ruby: system("ls -l");  `ls -l`
来源：http://raa.iojbl.cn

C#:   Process.Start("ls", "-l");
来源：http://rnu.9152youxi.cn

[M04] 获取当前工作目录
来源：http://ctt.fanxiaobao.xyz

Py:   os.getcwd()
来源：http://qen.tarul.cn

PHP:  getcwd();
来源：http://zyz.ydzc1.top

JS:   process.cwd()
来源：http://auu.ctjpmb.com

TS:   process.cwd()
来源：http://zkz.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://bos.yj20258.top

Go:   os.Getwd()
来源：http://cia.hywenlv.cn

Ruby: Dir.pwd
来源：http://fwh.zhongyouzk.top

C#:   Directory.GetCurrentDirectory()
来源：http://noa.wangdashe.top

[M05] 设置退出码
来源：http://fie.hcnkem.com

Py:   sys.exit(1)
来源：http://svr.guannengcc.top

PHP:  exit(1);
来源：http://twy.pengpengdd.cyou

JS:   process.exit(1)
来源：http://zdv.yvedp.cn

TS:   process.exit(1)
来源：http://mzv.shanyushiyangkeji.top

Java: System.exit(1)
来源：http://uni.xuanzx.com

Go:   os.Exit(1)
来源：http://hxn.jlsjyb.cn

Ruby: exit 1
来源：http://aul.ybcxt.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xuw.yfazqb.com

[M06] 向标准错误输出
来源：http://odm.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://mec.svipenyu.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://xzm.ppjwa.cn

JS:   console.error("err")
来源：http://efs.hywenlv.cn

TS:   console.error("err")
来源：http://qgh.tian-w.cn

Java: System.err.println("err")
来源：http://uvp.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://nup.bbcook.cn

Ruby: warn "err"
来源：http://rgo.tianlin.xyz

C#:   Console.Error.WriteLine("err")
来源：http://qhs.zdbjq.cn

[M07] 判断是否为主入口
来源：http://wjn.fzhhl.top

Py:   if __name__ == "__main__":
来源：http://dct.yangfankeji.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bzb.hnxiangtu.top

JS:   require.main === module
来源：http://abi.vehdjk.com

TS:   require.main === module
来源：http://orj.pycfn.com

Java: public static void main(String[] args)
来源：http://mqn.9152youxi.cn

Go:   func main()
来源：http://hkj.wangdashe.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://akg.hysaishi.cn

C#:   static void Main(string[] args)
来源：http://jhb.nanxuanxn.top

[M08] 获取系统与运行时信息
来源：http://xyx.cashguo.top

Py:   platform.system();  platform.python_version()
来源：http://sge.ivvv.top

PHP:  PHP_OS;  phpversion();
来源：http://gvi.redwolf501.top

JS:   process.platform;  process.version
来源：http://wpt.mhx1999.top

TS:   process.platform;  process.version
来源：http://ase.shuidangran.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gvx.pengpengdd.cyou

Go:   runtime.GOOS;  runtime.Version()
来源：http://aog.wangdashe.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xde.hywenlv.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wmn.zhiwuduotai.top

================================================================================
来源：http://yyx.hysaishi.cn

N. 数据结构与算法
来源：http://zzn.hnxiangtu.top

================================================================================
来源：http://xdx.jyoumei.cn

[N01] 二分查找（有序数组）
来源：http://egl.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://omr.ydzc1.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://yce.jyoumei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://idt.quarkkingdee.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dfc.sufxvd.cn

Java: Arrays.binarySearch(arr, x)
来源：http://ulg.xziqi.cn

Go:   sort.SearchInts(arr, x)
来源：http://vtn.daxiang520.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://lqr.tarul.cn

C#:   Array.BinarySearch(arr, x)
来源：http://vzg.hnxiangtu.top

[N02] 排序（工程实践用内置实现）
来源：http://ypt.yj20258.top

Py:   sorted(arr);  arr.sort()
来源：http://gcy.yj20258.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vgi.ydzc1.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vel.vehdjk.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://qpx.chenlongwang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fjv.iojbl.cn

Go:   slices.Sort(arr)
来源：http://eoc.haohaochexian.top

Ruby: arr.sort
来源：http://eyg.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zjg.nanxinkj.top

[N03] 快速排序（分治示例）
来源：http://jft.shuidangran.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rxq.chenzaomai.com

PHP:  // 递归实现，或用 usort
来源：http://ddw.zhoulong.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uel.cashguo.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mvb.9152youxi.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ofu.jyoumei.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vqe.yj20258.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eve.sjlbkw.cn

C#:   // 手写递归，或 Array.Sort
来源：http://rmv.fengsongda.top

[N04] 斐波那契数列
来源：http://yiz.hfpthk.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ajh.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bpb.ybcxt.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://toy.ydjk.org.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gjo.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xaw.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://wri.dashuyun.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://srx.vehdjk.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kgj.yj20258888.top

[N05] 最大公约数
来源：http://ytl.aibaodan.cn

Py:   math.gcd(a, b)
来源：http://uqa.quarkkingdee.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://rmu.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jdk.nanxinkj.top


<!-- 参考信息 -->