代发 wailian999

[J07] 比较两个日期
来源：http://weu.ydjk.org.cn

Py:   d1 < d2;  d1 == d2
来源：http://bba.zhixingplan.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://wmd.guannengcc.top

JS:   d1.getTime() < d2.getTime()
来源：http://zxw.hnqzz.top

TS:   d1.getTime() < d2.getTime()
来源：http://fmz.quarkkingdee.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://qzy.hcnkem.com

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://ocl.zhengqikj.top

Ruby: d1 < d2;  d1 == d2
来源：http://lld.yangfankeji.com

C#:   d1 < d2;  d1 == d2
来源：http://rjz.jyoumei.cn

[J08] 提取年月日与星期
来源：http://wwu.fzhhl.top

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://qtk.tanke756.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://akz.ctjpmb.com

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://igk.iojbl.cn

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://lul.wangdashe.top

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://hkg.0kj1m.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://emm.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://uoo.yfazqb.com

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://qnc.chenjidiqi.icu

[J09] 时区处理
来源：http://imx.yj202588.top

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://lwr.hcnkem.com

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://jyy.cheryme.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://xcj.ppjwa.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://jmh.gzhubu.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://mdq.yongpay.top

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://yba.nwbrower.top

Ruby: Time.now.getlocal("+08:00")
来源：http://zav.yj20258888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jfn.hysaishi.cn

[J10] 取今天 / 本月第一天
来源：http://xdi.hnqzz.top

Py:   date.today();  date.today().replace(day=1)
来源：http://tue.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://fgg.zhoulong.xyz

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://njr.ppjwa.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://cvy.tarul.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://skk.zhaomingkeji.xyz

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://dly.shanyushiyangkeji.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://yze.shzxlz.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ves.ydzc1.top

================================================================================
来源：http://qmd.aizwys.cn

K. JSON 与序列化
来源：http://ngg.aizwys.cn

================================================================================
来源：http://vlj.yj20258888.top

[K01] 对象转 JSON 字符串
来源：http://xeq.chenjidiqi.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://bxt.hfpthk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://yvu.shanyushiyangtech.top

JS:   JSON.stringify(obj)
来源：http://xgg.hesvh.cn

TS:   JSON.stringify(obj)
来源：http://kaz.hnqzz.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kps.cqqwz.cn

Go:   json.Marshal(obj)
来源：http://huy.ivvv.top

Ruby: obj.to_json                                     // require "json"
来源：http://qyr.jinqigfzy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://lwc.pycfn.com

[K02] JSON 字符串转对象
来源：http://xzo.uphjek.com

Py:   json.loads(s)
来源：http://unn.chenlongwang.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dqu.tian-w.cn

JS:   JSON.parse(s)
来源：http://lqv.tanke756.top

TS:   JSON.parse(s)
来源：http://snb.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rvu.hywenlv.cn

Go:   json.Unmarshal(data, &v)
来源：http://wkj.tarul.cn

Ruby: JSON.parse(s)
来源：http://gen.pengpengdd.cyou

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://sok.svipenyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://rje.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pkx.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://yvn.meibo888.top

JS:   JSON.stringify(obj, null, 2)
来源：http://zkl.chenjidiqi.icu

TS:   JSON.stringify(obj, null, 2)
来源：http://vnh.pengpengdd.cyou

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vsy.sjlbkw.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rip.feifeiyinyue.top

Ruby: JSON.pretty_generate(obj)
来源：http://cuo.mhx1999.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://zps.jinqigufen.top

[K04] 读取 JSON 文件
来源：http://rhu.uphjek.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fnm.ctjpmb.com

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xri.hcnkem.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vgw.xuetiantiany.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uhk.jlsjyb.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://zdk.dianchejie.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://pae.daria6918.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://krp.cheryme.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lxv.sweek.top

[K05] 深拷贝对象
来源：http://bwc.dianchejie.cn

Py:   copy.deepcopy(obj)
来源：http://xuk.zhongyouzk.top

PHP:  unserialize(serialize($obj));
来源：http://mck.wangshuangyany.cn

JS:   structuredClone(obj)
来源：http://kvt.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://ynn.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jtj.andypj.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tzy.zhongyouzk.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://zbv.hesvh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://crj.hywenlv.cn

[K06] 解析 URL 查询串
来源：http://fjq.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ahu.aibaodan.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://apj.zhixingplan.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ngx.jinghuilouyu.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zns.epnwcf.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://shg.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kht.fengsongda.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://yso.dashuyun.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://fqe.ydjk.org.cn

[K07] 进制转换
来源：http://jqq.pengpengdd.cyou

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bxa.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ixl.daxiang520.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://qyp.cashguo.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oki.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xxs.ehwqpu.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pei.hnqzz.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lfg.ywan-chungtsiang.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fqz.zhixingplan.top

[K08] 二进制序列化（非 JSON）
来源：http://qhk.hnqzz.top

Py:   pickle.dumps(obj)
来源：http://pce.shanyushiyangtech.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nne.zhaomingkeji.xyz

JS:   v8.serialize(obj)        // Node
来源：http://jhz.dashuyun.cn

TS:   v8.serialize(obj)        // Node
来源：http://yni.zycfv.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://tvx.sufxvd.cn

Go:   encoding/gob
来源：http://isd.zhijiandao.cn

Ruby: Marshal.dump(obj)
来源：http://gnk.svipenyu.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dgc.ydzc1.top

================================================================================
来源：http://nch.xuetiantiany.cn

L. 网络请求
来源：http://lpw.hfpthk.cn

================================================================================
来源：http://aju.chenzaomai.com

[L01] 发送 GET 请求
来源：http://kpo.fengsongda.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rgq.meibo888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://oro.chenjidiqi.icu

JS:   await fetch(url)
来源：http://ldu.sweek.top

TS:   await fetch(url)
来源：http://cai.xuanzx.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://lyl.guowangkeji.top

Go:   resp, err := http.Get(url)
来源：http://nai.shanyushiyangkeji.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oey.shanyushiyangtech.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kkm.zycfv.cn

[L02] 发送 POST JSON
来源：http://yed.yuanzhike.top

Py:   requests.post(url, json={"a": 1})
来源：http://bus.cdnleiting.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://usq.smart0.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ktz.zhengqikj.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rkm.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ash.zhongyouzk.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://jbp.yuanzhike.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://dmo.shanyushiyangtech.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bdf.yj20258888.top

[L03] 设置自定义请求头
来源：http://doa.chenzaomai.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://rys.jinqigufen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dhf.xziqi.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xlz.cheryme.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fmb.cheryme.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://xyp.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://qfm.9152youxi.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://gdb.ctjpmb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://osi.jinghuilouyu.cn

[L04] 设置超时
来源：http://lvd.jqgfzy.top

Py:   requests.get(url, timeout=5)
来源：http://ede.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://emg.yfazqb.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://upo.yfazqb.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bkz.shanyushiyangkeji.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://slk.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pcg.chenjidiqi.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cci.hcnkem.com

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://svx.jinqigufen.top

[L05] 上传文件（multipart）
来源：http://eux.jlsjyb.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eqt.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zlg.chenjidiqi.icu

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://jpf.redwolf501.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://qvl.daria6918.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mtx.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bfp.sweek.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zql.dashuyun.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://kuk.nwbrower.top

[L06] 解析响应为 JSON
来源：http://apu.vehdjk.com

Py:   resp.json()
来源：http://hfd.mhx1999.top

PHP:  json_decode($body, true);
来源：http://ptw.ydjk.org.cn

JS:   await resp.json()
来源：http://pjz.yj202588.top

TS:   await resp.json()
来源：http://kfn.wangdashe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ndd.fktsv.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ojo.shanyushiyangtech.top

Ruby: JSON.parse(resp.body)
来源：http://xjo.ybcxt.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mry.tarul.cn

[L07] 处理 HTTP 状态码
来源：http://kdw.haohaochexian.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mnf.dianchejie.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://hxh.shzxlz.cn

JS:   resp.ok;  resp.status
来源：http://wzl.tanke756.top

TS:   resp.ok;  resp.status
来源：http://tmi.zdqjudy.top

Java: resp.statusCode()
来源：http://zek.yuxming.cn

Go:   resp.StatusCode
来源：http://bus.nanxinkj.top

Ruby: resp.code.to_i
来源：http://sdr.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://uua.hesvh.cn

[L08] 并发请求多个地址
来源：http://mur.ctjpmb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tif.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://aek.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://buo.ivvv.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ywz.nwbrower.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://piq.guowangkeji.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ovj.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sop.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ind.zhixingplan.top

================================================================================
来源：http://yqd.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://nuj.ybcxt.top

================================================================================
来源：http://mqt.xuetiantiany.cn

[M01] 读取命令行参数
来源：http://lqw.quarkkingdee.top

Py:   sys.argv[1:]
来源：http://brg.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://pww.kuanghao11.cn

JS:   process.argv.slice(2)
来源：http://pxd.sjlbkw.cn

TS:   process.argv.slice(2)
来源：http://dnt.pycfn.com

Java: args 数组（main 方法参数）
来源：http://bto.cucudq.cn

Go:   os.Args[1:]
来源：http://vfv.cucudq.cn

Ruby: ARGV
来源：http://kwn.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://ygo.snrcjt.cn

[M02] 读取环境变量
来源：http://izf.havefunace.top

Py:   os.environ.get("HOME")
来源：http://ric.tanke756.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://nnk.fengsongda.top

JS:   process.env.HOME
来源：http://jhx.hcnkem.com

TS:   process.env.HOME
来源：http://dwz.zhixingplan.top

Java: System.getenv("HOME")
来源：http://yiy.52xcode.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://cid.chenlongwang.top

Ruby: ENV["HOME"]
来源：http://fql.sjlbkw.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bop.yueranfly.top

[M03] 执行外部命令
来源：http://pid.mhx1999.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://hdd.yj20258.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jwq.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://twb.jqgfzy.top

TS:   child_process.execSync("ls -l").toString()
来源：http://qls.quarkkingdee.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gdt.vqdsnc.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://gpw.aizwys.cn

Ruby: system("ls -l");  `ls -l`
来源：http://nsx.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://bof.xinyue.icu

[M04] 获取当前工作目录
来源：http://zjx.mhx1999.top

Py:   os.getcwd()
来源：http://dfj.hongshengwenyu.top

PHP:  getcwd();
来源：http://loz.daxiang520.top

JS:   process.cwd()
来源：http://phr.sweek.top

TS:   process.cwd()
来源：http://zsv.xuanzx.com

Java: Path.of("").toAbsolutePath()
来源：http://lhy.gzhubu.top

Go:   os.Getwd()
来源：http://ali.hysaishi.cn

Ruby: Dir.pwd
来源：http://qyk.sufxvd.cn

C#:   Directory.GetCurrentDirectory()
来源：http://foc.xziqi.cn

[M05] 设置退出码
来源：http://fxu.gzhubu.top

Py:   sys.exit(1)
来源：http://kry.zhijiandao.cn

PHP:  exit(1);
来源：http://yzb.fengsongda.top

JS:   process.exit(1)
来源：http://iav.zhaomingkeji.xyz

TS:   process.exit(1)
来源：http://itv.cashguo.top

Java: System.exit(1)
来源：http://jge.iojbl.cn

Go:   os.Exit(1)
来源：http://imx.kuanghao11.cn

Ruby: exit 1
来源：http://aij.jinyuanbaomall.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://cub.ybcxt.top

[M06] 向标准错误输出
来源：http://vkw.xinyue.icu

Py:   print("err", file=sys.stderr)
来源：http://wzx.nanxuanxn.top

PHP:  fwrite(STDERR, "err\n");
来源：http://bhx.wangshuangyany.cn

JS:   console.error("err")
来源：http://dqv.xuanzx.com

TS:   console.error("err")
来源：http://uaj.sjlbkw.cn

Java: System.err.println("err")
来源：http://nyh.gzhubu.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://rop.uphjek.com

Ruby: warn "err"
来源：http://nuh.yuanzhike.top

C#:   Console.Error.WriteLine("err")
来源：http://lwd.zhengqikj.top

[M07] 判断是否为主入口
来源：http://ozn.sjlbkw.cn

Py:   if __name__ == "__main__":
来源：http://ued.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kbd.gzhubu.top

JS:   require.main === module
来源：http://gtc.jinghuilouyu.cn

TS:   require.main === module
来源：http://oei.feifeiyinyue.top

Java: public static void main(String[] args)
来源：http://qba.gaohongyu789.top

Go:   func main()
来源：http://vrd.daria6918.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mun.hongshengwenyu.top

C#:   static void Main(string[] args)
来源：http://azp.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://ztx.cqqwz.cn

Py:   platform.system();  platform.python_version()
来源：http://kwv.xuanzx.com

PHP:  PHP_OS;  phpversion();
来源：http://snq.yangfankeji.com

JS:   process.platform;  process.version
来源：http://nwz.daxiang520.top

TS:   process.platform;  process.version
来源：http://hmx.uphjek.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://gcg.mhx1999.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ssu.aibaodan.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cgl.fzhhl.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://fqq.svipenyu.cn

================================================================================
来源：http://acc.yonumen.top

N. 数据结构与算法
来源：http://txe.shangyingyoupin.top

================================================================================
来源：http://jkr.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://owj.hammf.cn

Py:   bisect.bisect_left(arr, x)
来源：http://pkb.shangyingyoupin.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rgx.hysaishi.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wzc.fengsongda.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vhb.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dbl.aizwys.cn

Go:   sort.SearchInts(arr, x)
来源：http://kvj.chenzaomai.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://mvq.feifeiyinyue.top

C#:   Array.BinarySearch(arr, x)
来源：http://dyb.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://jjg.xuetiantiany.cn

Py:   sorted(arr);  arr.sort()
来源：http://wun.quarkkingdee.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://mms.ywan-chungtsiang.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://aeu.zhiwuduotai.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://egk.zhaomingkeji.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pzn.gaohongyu789.top

Go:   slices.Sort(arr)
来源：http://xir.yonumen.top

Ruby: arr.sort
来源：http://iwi.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yvy.hesvh.cn

[N03] 快速排序（分治示例）
来源：http://coo.jlsjyb.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ced.bjfxy.top

PHP:  // 递归实现，或用 usort
来源：http://tjk.cdnleiting.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rkq.tarul.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sbu.52xcode.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://puv.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://sve.svipenyu.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://njt.tanke756.top

C#:   // 手写递归，或 Array.Sort
来源：http://zhl.yfazqb.com

[N04] 斐波那契数列
来源：http://npx.haohaochexian.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://tul.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kki.zhijiandao.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dxq.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cco.daxiang520.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://rrm.jlsjyb.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mvu.c1oappe.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zrb.tian-w.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dhz.zhaomingkeji.xyz


<!-- 参考信息 -->