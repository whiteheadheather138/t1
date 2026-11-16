代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://mql.xylfe.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://vyr.yuanzhike.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://juc.nanxinkj.top

[J10] 取今天 / 本月第一天
来源：http://uqp.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://bhq.pycfn.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://vvv.dianchejie.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://kkg.hysaishi.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mth.iojbl.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hgj.hfpthk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kug.nanxinkj.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bnl.guannengcc.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rrr.gotoacloud.top

================================================================================
来源：http://xod.gaohongyu789.top

K. JSON 与序列化
来源：http://lml.hnxiangtu.top

================================================================================
来源：http://kng.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://eat.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ruc.zhijiandao.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://qyx.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://ynw.zhongyouzk.top

TS:   JSON.stringify(obj)
来源：http://tpi.cheryme.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kks.vqdsnc.cn

Go:   json.Marshal(obj)
来源：http://mmu.zhixingplan.top

Ruby: obj.to_json                                     // require "json"
来源：http://iah.yuxming.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://zks.ivvv.top

[K02] JSON 字符串转对象
来源：http://kzk.gogol.net.cn

Py:   json.loads(s)
来源：http://rel.cheryme.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://pby.jyoumei.cn

JS:   JSON.parse(s)
来源：http://cya.cheryme.top

TS:   JSON.parse(s)
来源：http://qwf.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://qop.zhixingplan.top

Go:   json.Unmarshal(data, &v)
来源：http://yot.iojbl.cn

Ruby: JSON.parse(s)
来源：http://max.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://uzs.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://jkc.gogol.net.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://heq.cucudq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://miu.hysaishi.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://dsd.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://bmg.yongpay.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bbl.hongshengwenyu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kbw.c1oappe.top

Ruby: JSON.pretty_generate(obj)
来源：http://ypc.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jhd.gotoacloud.top

[K04] 读取 JSON 文件
来源：http://sog.yongpay.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ytb.aibaodan.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gfu.quarkkingdee.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lez.sufxvd.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cks.ivvv.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://hvo.chenjidiqi.icu

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gtu.316326.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://jrk.yfazqb.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://icd.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://kup.vqdsnc.cn

Py:   copy.deepcopy(obj)
来源：http://qjj.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://cik.jinqigufen.top

JS:   structuredClone(obj)
来源：http://fmv.zycfv.cn

TS:   structuredClone(obj)
来源：http://dpv.xylfe.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://mhb.0kj1m.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qrr.iojbl.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kzv.ehwqpu.com

C#:   // 序列化往返，或自定义 Clone
来源：http://jov.meibo888.top

[K06] 解析 URL 查询串
来源：http://oir.zhixingplan.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://eau.yangfankeji.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hmj.jiagoushi.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://adw.yj20258888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cln.daxiang520.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://plr.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://dnx.xuetiantiany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ylk.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zxh.cdnleiting.top

[K07] 进制转换
来源：http://tfz.uphjek.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://clb.dianchejie.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ozl.daria6918.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bnh.ehwqpu.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://olj.jinghuilouyu.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://owa.fehbvm.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://dqa.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://uge.zdqjudy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ceb.fehbvm.com

[K08] 二进制序列化（非 JSON）
来源：http://zbc.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://ngg.jinqigufen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zbt.wangshuangyany.cn

JS:   v8.serialize(obj)        // Node
来源：http://xyp.svipenyu.cn

TS:   v8.serialize(obj)        // Node
来源：http://ojd.jinghuilouyu.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eym.dashuyun.cn

Go:   encoding/gob
来源：http://zrr.kuanghao11.cn

Ruby: Marshal.dump(obj)
来源：http://yyh.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rud.ehwqpu.com

================================================================================
来源：http://gof.tarul.cn

L. 网络请求
来源：http://png.ywan-chungtsiang.top

================================================================================
来源：http://hxj.zhijiandao.cn

[L01] 发送 GET 请求
来源：http://cxa.wangdashe.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ebl.jianghu66.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rjd.fengsongda.top

JS:   await fetch(url)
来源：http://nip.hesvh.cn

TS:   await fetch(url)
来源：http://rkc.vqdsnc.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://fbs.fktsv.cn

Go:   resp, err := http.Get(url)
来源：http://ikj.tianlin.xyz

Ruby: Net::HTTP.get(URI(url))
来源：http://tpu.aibaodan.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ake.snrcjt.cn

[L02] 发送 POST JSON
来源：http://lri.svipenyu.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fib.gotoacloud.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zjr.yonumen.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vxm.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://osn.vqdsnc.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kop.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://aix.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://qrt.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://qaq.hnqzz.top

[L03] 设置自定义请求头
来源：http://qqu.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://efx.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vzr.chenjidiqi.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xqb.ppjwa.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vyh.ydzc1.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://syo.sweek.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://mxa.zhoulong.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://auv.zhijiandao.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jfa.zdbjq.cn

[L04] 设置超时
来源：http://tii.dianchejie.cn

Py:   requests.get(url, timeout=5)
来源：http://mob.zhiwuduotai.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://voq.hesvh.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nqw.aibaodan.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uki.svipenyu.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wyl.shanyushiyangtech.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bnp.yanxiufei.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://scf.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://amw.yj20258.top

[L05] 上传文件（multipart）
来源：http://ghn.haohaochexian.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xpl.ctjpmb.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zgf.yongpay.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ohm.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bpm.guannengcc.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qtu.wangshuangyany.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cul.ppjwa.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://udd.andypj.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fmv.fehbvm.com

[L06] 解析响应为 JSON
来源：http://bln.hywenlv.cn

Py:   resp.json()
来源：http://acy.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://hiq.pengpengdd.cyou

JS:   await resp.json()
来源：http://quz.hywenlv.cn

TS:   await resp.json()
来源：http://jyj.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jsr.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vkr.hnqzz.top

Ruby: JSON.parse(resp.body)
来源：http://wsq.yangfankeji.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ztb.tian-w.cn

[L07] 处理 HTTP 状态码
来源：http://kqg.gzhubu.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://kxz.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://trh.fengsongda.top

JS:   resp.ok;  resp.status
来源：http://ykw.jinghuilouyu.cn

TS:   resp.ok;  resp.status
来源：http://xok.uphjek.com

Java: resp.statusCode()
来源：http://eyv.ehwqpu.com

Go:   resp.StatusCode
来源：http://gjt.svipenyu.cn

Ruby: resp.code.to_i
来源：http://amr.ybcxt.top

C#:   (int)resp.StatusCode
来源：http://yce.sufxvd.cn

[L08] 并发请求多个地址
来源：http://cbg.vehdjk.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nzi.316326.xyz

PHP:  curl_multi_init() 系列
来源：http://qyr.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eav.zdbjq.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://utp.pycfn.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://usj.bbcook.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zhy.snrcjt.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://prz.yanxiufei.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ily.quarkkingdee.top

================================================================================
来源：http://mpk.yueranfly.top

M. 命令行 / 进程 / 环境
来源：http://ibv.yanxiufei.cn

================================================================================
来源：http://irv.aizwys.cn

[M01] 读取命令行参数
来源：http://zbm.zhaomingkeji.xyz

Py:   sys.argv[1:]
来源：http://hnd.daxiang520.top

PHP:  $argv;  $argc;
来源：http://qca.xylfe.cn

JS:   process.argv.slice(2)
来源：http://lod.vqdsnc.cn

TS:   process.argv.slice(2)
来源：http://vjy.bjfxy.top

Java: args 数组（main 方法参数）
来源：http://qio.yongpay.top

Go:   os.Args[1:]
来源：http://fme.cashguo.top

Ruby: ARGV
来源：http://lxt.sxryk.cn

C#:   args 数组（Main 方法参数）
来源：http://lwv.cheryme.top

[M02] 读取环境变量
来源：http://igp.sxryk.cn

Py:   os.environ.get("HOME")
来源：http://bkh.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dga.fengsongda.top

JS:   process.env.HOME
来源：http://syb.fengsongda.top

TS:   process.env.HOME
来源：http://lek.fktsv.cn

Java: System.getenv("HOME")
来源：http://afe.hcnkem.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lbr.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://kri.gzhubu.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://kee.meibo888.top

[M03] 执行外部命令
来源：http://qyg.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://irn.redwolf501.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://czs.ydzc1.top

JS:   child_process.execSync("ls -l").toString()
来源：http://vrw.xylfe.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://bou.hywenlv.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://tqk.chenjidiqi.icu

Go:   exec.Command("ls", "-l").Output()
来源：http://hao.bjfxy.top

Ruby: system("ls -l");  `ls -l`
来源：http://zxu.fanxiaobao.xyz

C#:   Process.Start("ls", "-l");
来源：http://kkg.ydjk.org.cn

[M04] 获取当前工作目录
来源：http://eqo.fengsongda.top

Py:   os.getcwd()
来源：http://obw.yongpay.top

PHP:  getcwd();
来源：http://ejd.hysaishi.cn

JS:   process.cwd()
来源：http://bpb.jinghuilouyu.cn

TS:   process.cwd()
来源：http://csy.cashguo.top

Java: Path.of("").toAbsolutePath()
来源：http://pcb.fengsongda.top

Go:   os.Getwd()
来源：http://pwg.zhoulong.xyz

Ruby: Dir.pwd
来源：http://xiw.jlsjyb.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wlm.jiagoushi.top

[M05] 设置退出码
来源：http://bax.chenzaomai.com

Py:   sys.exit(1)
来源：http://hus.gaohongyu789.top

PHP:  exit(1);
来源：http://yad.gotoacloud.top

JS:   process.exit(1)
来源：http://fau.nwbrower.top

TS:   process.exit(1)
来源：http://fdl.jianghu66.top

Java: System.exit(1)
来源：http://nrd.sjlbkw.cn

Go:   os.Exit(1)
来源：http://anm.zycfv.cn

Ruby: exit 1
来源：http://ubx.smart0.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xpv.wangshuangyany.cn

[M06] 向标准错误输出
来源：http://cue.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://xms.haohaochexian.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sqb.ehwqpu.com

JS:   console.error("err")
来源：http://mmn.smart0.xyz

TS:   console.error("err")
来源：http://exx.jqgfzy.top

Java: System.err.println("err")
来源：http://yid.cdnleiting.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hjk.cqqwz.cn

Ruby: warn "err"
来源：http://zyl.guowangkeji.top

C#:   Console.Error.WriteLine("err")
来源：http://hoh.zhiwuduotai.top

[M07] 判断是否为主入口
来源：http://nsj.hongshengwenyu.top

Py:   if __name__ == "__main__":
来源：http://fka.fzhhl.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kwd.hywenlv.cn

JS:   require.main === module
来源：http://edp.jinqigufen.top

TS:   require.main === module
来源：http://iiz.0kj1m.cn

Java: public static void main(String[] args)
来源：http://wtg.9152youxi.cn

Go:   func main()
来源：http://suw.hnqzz.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eio.andypj.xyz

C#:   static void Main(string[] args)
来源：http://waq.cdnleiting.top

[M08] 获取系统与运行时信息
来源：http://xtp.xingfuxueyuan.xyz

Py:   platform.system();  platform.python_version()
来源：http://wfc.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://pux.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://drt.gogol.net.cn

TS:   process.platform;  process.version
来源：http://snl.hnqzz.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oyn.yj202588.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://hyb.nanxinkj.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vsb.hnxiangtu.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ozs.cucudq.cn

================================================================================
来源：http://lft.jqgufenzy.top

N. 数据结构与算法
来源：http://qom.yj20258888.top

================================================================================
来源：http://ihh.gaohongyu789.top

[N01] 二分查找（有序数组）
来源：http://lsh.jqgufenzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://ddf.jqgufenzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://ski.andypj.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ypl.jinyuanbaomall.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eej.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://rpr.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://hjp.jqgufenzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://htt.cucudq.cn

C#:   Array.BinarySearch(arr, x)
来源：http://dgr.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://rvm.gzhubu.top

Py:   sorted(arr);  arr.sort()
来源：http://nnl.gogol.net.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qtz.zhixingplan.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qka.dianchejie.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hgc.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vlt.aibaodan.cn

Go:   slices.Sort(arr)
来源：http://mrs.dashuyun.cn

Ruby: arr.sort
来源：http://awt.gaohongyu789.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://xuj.yuxming.cn

[N03] 快速排序（分治示例）
来源：http://boq.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sss.xingfuxueyuan.xyz

PHP:  // 递归实现，或用 usort
来源：http://jpo.yuxming.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uop.hcnkem.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://axm.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://drm.hesvh.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ujk.wangshuangyany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ijv.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://kqn.cucudq.cn

[N04] 斐波那契数列
来源：http://xma.snrcjt.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://kts.dashuyun.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ubl.mhx1999.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rgm.fktsv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eyt.sweek.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qud.guowangkeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://edg.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vwx.chenlongwang.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gcm.nanxuanxn.top

[N05] 最大公约数
来源：http://abl.cdnleiting.top

Py:   math.gcd(a, b)
来源：http://pcz.ivvv.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jyt.wangshuangyany.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://onl.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ito.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://xvf.andypj.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://yrh.hongshengwenyu.top

Ruby: a.gcd(b)
来源：http://fwn.yueranfly.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lfl.snrcjt.cn

[N06] 判断回文字符串
来源：http://asm.cashguo.top

Py:   s == s[::-1]
来源：http://iyg.cqqwz.cn

PHP:  $s === strrev($s);
来源：http://cvl.snrcjt.cn

JS:   s === [...s].reverse().join("")
来源：http://rup.yueranfly.top

TS:   s === [...s].reverse().join("")
来源：http://xiy.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://oom.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://mlv.jiagoushi.top

Ruby: s == s.reverse
来源：http://wrg.xingfuxueyuan.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://age.tarul.cn

[N07] 两数之和（返回下标）
来源：http://oxm.yj20258888.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ukr.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kvu.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://beo.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://pif.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://lcs.hnqzz.top


<!-- 参考信息 -->