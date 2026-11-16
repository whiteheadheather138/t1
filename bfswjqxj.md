代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://kwm.shzxlz.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://obp.guowangkeji.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://pur.yfazqb.com

[J10] 取今天 / 本月第一天
来源：http://iuc.sxryk.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://quu.wangdashe.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://hwr.jinyuanbaomall.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://zbc.hammf.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://mnp.ybcxt.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://crm.meibo888.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bow.jinqigfzy.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://nqs.yuxming.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xgl.hywenlv.cn

================================================================================
来源：http://uaq.shangyingyoupin.top

K. JSON 与序列化
来源：http://enj.smart0.xyz

================================================================================
来源：http://aew.gzhubu.top

[K01] 对象转 JSON 字符串
来源：http://ncy.vehdjk.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://afv.fengsongda.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tpy.fktsv.cn

JS:   JSON.stringify(obj)
来源：http://hhn.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://tnc.yuanzhike.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ima.fengsongda.top

Go:   json.Marshal(obj)
来源：http://zdr.shuidangran.top

Ruby: obj.to_json                                     // require "json"
来源：http://ywt.zhijiandao.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fbr.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://syh.ctjpmb.com

Py:   json.loads(s)
来源：http://qcb.sysykeji.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qmn.gaohongyu789.top

JS:   JSON.parse(s)
来源：http://ksa.jiagoushi.top

TS:   JSON.parse(s)
来源：http://bjk.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://reo.hammf.cn

Go:   json.Unmarshal(data, &v)
来源：http://dkr.52xcode.cn

Ruby: JSON.parse(s)
来源：http://lye.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wyg.mhx1999.top

[K03] JSON 美化输出（带缩进）
来源：http://mmy.jyoumei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ivv.fktsv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://buc.cucudq.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://huu.tian-w.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xth.zhaomingkeji.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://sex.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://arv.zhengqikj.top

Ruby: JSON.pretty_generate(obj)
来源：http://yis.yongpay.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ekb.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://the.c1oappe.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jzz.pengpengdd.cyou

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://fho.ydjk.org.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dsi.hammf.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pbl.jqgfzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qhd.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ybe.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://xyz.uphjek.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ojl.cqqwz.cn

[K05] 深拷贝对象
来源：http://hyu.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://zxc.cashguo.top

PHP:  unserialize(serialize($obj));
来源：http://vqu.ehwqpu.com

JS:   structuredClone(obj)
来源：http://oue.hongshengwenyu.top

TS:   structuredClone(obj)
来源：http://tgl.daxiang520.top

Java: // 手写拷贝构造，或序列化往返
来源：http://hfa.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://mms.jqgfzy.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uxl.nanxinkj.top

C#:   // 序列化往返，或自定义 Clone
来源：http://dca.wangdashe.top

[K06] 解析 URL 查询串
来源：http://qdu.hammf.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fsd.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://uwo.yangfankeji.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bvm.xziqi.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://win.meibo888.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://umg.0kj1m.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://oav.pengpengdd.cyou

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nrr.xinyue.icu

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yzm.sufxvd.cn

[K07] 进制转换
来源：http://kvx.yanxiufei.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dwr.gzhubu.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://qgx.yfazqb.com

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mcp.cheryme.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://loo.andypj.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://xnx.jyoumei.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jge.redwolf501.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ifv.xinyue.icu

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://vyj.jyoumei.cn

[K08] 二进制序列化（非 JSON）
来源：http://qvo.vehdjk.com

Py:   pickle.dumps(obj)
来源：http://mqu.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qcs.shanyushiyangtech.top

JS:   v8.serialize(obj)        // Node
来源：http://pfz.chenlongwang.top

TS:   v8.serialize(obj)        // Node
来源：http://opw.nanxuanxn.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mvk.jqgfzy.top

Go:   encoding/gob
来源：http://yjr.epnwcf.com

Ruby: Marshal.dump(obj)
来源：http://onr.tarul.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kcu.uphjek.com

================================================================================
来源：http://cqm.yangfankeji.com

L. 网络请求
来源：http://yal.zhoulong.xyz

================================================================================
来源：http://vpp.shzxlz.cn

[L01] 发送 GET 请求
来源：http://bzo.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://acq.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rcr.yj202588.top

JS:   await fetch(url)
来源：http://our.hammf.cn

TS:   await fetch(url)
来源：http://tbc.kuanghao11.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://srq.aizwys.cn

Go:   resp, err := http.Get(url)
来源：http://gtz.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://xlh.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kvm.dianchejie.cn

[L02] 发送 POST JSON
来源：http://auj.feifeiyinyue.top

Py:   requests.post(url, json={"a": 1})
来源：http://egq.zdbjq.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ggc.c1oappe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://grx.yj202588.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wvg.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://uun.fktsv.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://gga.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://npf.yuanzhike.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jtt.hnqzz.top

[L03] 设置自定义请求头
来源：http://wjy.guowangkeji.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jjk.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://smt.hcnkem.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cpa.zhixingplan.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dks.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wxk.kuanghao11.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hji.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ogx.jinqigufen.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://uys.uphjek.com

[L04] 设置超时
来源：http://jvc.jianghu66.top

Py:   requests.get(url, timeout=5)
来源：http://cbm.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://swb.jqgufenzy.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://loi.fanxiaobao.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wzy.zhoulong.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ndd.hnxiangtu.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://ost.jiagoushi.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://cmp.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bgv.vehdjk.com

[L05] 上传文件（multipart）
来源：http://ovl.nwbrower.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dqj.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lyc.hesvh.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://svu.xziqi.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://mmz.sjlbkw.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://har.hesvh.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://vkm.shanyushiyangkeji.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://lvr.jinqigufen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wvt.ydjk.org.cn

[L06] 解析响应为 JSON
来源：http://xow.svipenyu.cn

Py:   resp.json()
来源：http://etv.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://fgs.tian-w.cn

JS:   await resp.json()
来源：http://smb.zhiwuduotai.top

TS:   await resp.json()
来源：http://shj.ppjwa.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://bae.iojbl.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mlz.tian-w.cn

Ruby: JSON.parse(resp.body)
来源：http://owy.0kj1m.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://cem.ivvv.top

[L07] 处理 HTTP 状态码
来源：http://iqw.cashguo.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://nyo.zdbjq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://mmo.kuanghao11.cn

JS:   resp.ok;  resp.status
来源：http://uss.shanyushiyangkeji.top

TS:   resp.ok;  resp.status
来源：http://tcg.tianlin.xyz

Java: resp.statusCode()
来源：http://scs.iojbl.cn

Go:   resp.StatusCode
来源：http://uqy.jinyuanbaomall.cn

Ruby: resp.code.to_i
来源：http://iab.sweek.top

C#:   (int)resp.StatusCode
来源：http://vwk.yueranfly.top

[L08] 并发请求多个地址
来源：http://uxo.yuanzhike.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tyi.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://ysi.yonumen.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://byf.fanxiaobao.xyz

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fbx.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uic.daria6918.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://soc.ctjpmb.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://enz.jinghuilouyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://oow.sweek.top

================================================================================
来源：http://tzb.fanxiaobao.xyz

M. 命令行 / 进程 / 环境
来源：http://jkc.shangyingyoupin.top

================================================================================
来源：http://ulu.yj20258888.top

[M01] 读取命令行参数
来源：http://wfb.kuanghao11.cn

Py:   sys.argv[1:]
来源：http://jhm.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://oho.zhongyouzk.top

JS:   process.argv.slice(2)
来源：http://zsk.cashguo.top

TS:   process.argv.slice(2)
来源：http://azj.nanxinkj.top

Java: args 数组（main 方法参数）
来源：http://pnq.xinyue.icu

Go:   os.Args[1:]
来源：http://wff.hesvh.cn

Ruby: ARGV
来源：http://xhx.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://heg.meibo888.top

[M02] 读取环境变量
来源：http://stc.tianlin.xyz

Py:   os.environ.get("HOME")
来源：http://wdc.tianlin.xyz

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://eor.wangshuangyany.cn

JS:   process.env.HOME
来源：http://yhh.xylfe.cn

TS:   process.env.HOME
来源：http://wkk.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://gfx.yanxiufei.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ozb.ybcxt.top

Ruby: ENV["HOME"]
来源：http://dgq.hesvh.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ojp.52xcode.cn

[M03] 执行外部命令
来源：http://kxi.bbcook.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wmx.ctjpmb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xaz.daxiang520.top

JS:   child_process.execSync("ls -l").toString()
来源：http://iln.sxryk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xlb.tian-w.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://had.ppjwa.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://npp.ybcxt.top

Ruby: system("ls -l");  `ls -l`
来源：http://qxe.xziqi.cn

C#:   Process.Start("ls", "-l");
来源：http://mhj.yonumen.top

[M04] 获取当前工作目录
来源：http://mob.pycfn.com

Py:   os.getcwd()
来源：http://hbl.chenjidiqi.icu

PHP:  getcwd();
来源：http://pig.jlsjyb.cn

JS:   process.cwd()
来源：http://ibq.ydjk.org.cn

TS:   process.cwd()
来源：http://haz.dashuyun.cn

Java: Path.of("").toAbsolutePath()
来源：http://ual.jiagoushi.top

Go:   os.Getwd()
来源：http://qex.jinghuilouyu.cn

Ruby: Dir.pwd
来源：http://vqe.c1oappe.top

C#:   Directory.GetCurrentDirectory()
来源：http://udf.52xcode.cn

[M05] 设置退出码
来源：http://lzw.fengsongda.top

Py:   sys.exit(1)
来源：http://aok.cqqwz.cn

PHP:  exit(1);
来源：http://ddz.haohaochexian.top

JS:   process.exit(1)
来源：http://stn.guannengcc.top

TS:   process.exit(1)
来源：http://esq.zdqjudy.top

Java: System.exit(1)
来源：http://wkl.yj202588.top

Go:   os.Exit(1)
来源：http://bnk.yj20258888.top

Ruby: exit 1
来源：http://moq.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://aua.xinyue.icu

[M06] 向标准错误输出
来源：http://gay.0kj1m.cn

Py:   print("err", file=sys.stderr)
来源：http://tmj.tianlin.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://gvm.hcnkem.com

JS:   console.error("err")
来源：http://iqm.xziqi.cn

TS:   console.error("err")
来源：http://jwu.chenlongwang.top

Java: System.err.println("err")
来源：http://qvd.ctjpmb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lya.smart0.xyz

Ruby: warn "err"
来源：http://nxx.fanxiaobao.xyz

C#:   Console.Error.WriteLine("err")
来源：http://xwt.jqgufenzy.top

[M07] 判断是否为主入口
来源：http://pmk.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://fvr.jyoumei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bqp.gotoacloud.top

JS:   require.main === module
来源：http://pct.hnxiangtu.top

TS:   require.main === module
来源：http://dvc.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://cms.jinghuilouyu.cn

Go:   func main()
来源：http://tll.zdqjudy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bgy.9152youxi.cn

C#:   static void Main(string[] args)
来源：http://ilv.xziqi.cn

[M08] 获取系统与运行时信息
来源：http://ptr.fehbvm.com

Py:   platform.system();  platform.python_version()
来源：http://urb.cucudq.cn

PHP:  PHP_OS;  phpversion();
来源：http://zrb.xziqi.cn

JS:   process.platform;  process.version
来源：http://rgv.hfpthk.cn

TS:   process.platform;  process.version
来源：http://vwt.aibaodan.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wgl.snrcjt.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://otw.ydzc1.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ujg.jqgufenzy.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://llg.mhx1999.top

================================================================================
来源：http://jkw.zhiwuduotai.top

N. 数据结构与算法
来源：http://oer.gzhubu.top

================================================================================
来源：http://igo.cdnleiting.top

[N01] 二分查找（有序数组）
来源：http://wtm.daria6918.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zoh.shuidangran.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rqu.uphjek.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gnn.ivvv.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ron.ppjwa.cn

Java: Arrays.binarySearch(arr, x)
来源：http://lpc.hysaishi.cn

Go:   sort.SearchInts(arr, x)
来源：http://fly.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://moq.316326.xyz

C#:   Array.BinarySearch(arr, x)
来源：http://kea.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://avd.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://dte.jqgfzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nrs.shuidangran.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://gnu.xuetiantiany.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://bsa.xylfe.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ane.bjfxy.top

Go:   slices.Sort(arr)
来源：http://osn.mhx1999.top

Ruby: arr.sort
来源：http://jtu.sxryk.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://msj.zhixingplan.top

[N03] 快速排序（分治示例）
来源：http://vlz.bbcook.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fky.gotoacloud.top

PHP:  // 递归实现，或用 usort
来源：http://noa.ybcxt.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iik.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://kly.fanxiaobao.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zls.wangshuangyany.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://pbv.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://mlq.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://gxe.316326.xyz

[N04] 斐波那契数列
来源：http://ovd.cheryme.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ngj.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ist.bjfxy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://pjy.daxiang520.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qpl.havefunace.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nly.sysykeji.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fzv.cdnleiting.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://okr.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://zue.meibo888.top

[N05] 最大公约数
来源：http://unq.dashuyun.cn

Py:   math.gcd(a, b)
来源：http://tjo.sysykeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://nzs.andypj.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pyi.ppjwa.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ork.xziqi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fcd.yuanzhike.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ywn.ydjk.org.cn

Ruby: a.gcd(b)
来源：http://fwp.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bfy.zhixingplan.top

[N06] 判断回文字符串
来源：http://moq.birdmap.top

Py:   s == s[::-1]
来源：http://yct.nanxinkj.top

PHP:  $s === strrev($s);
来源：http://wix.tian-w.cn

JS:   s === [...s].reverse().join("")
来源：http://kfv.yanxiufei.cn

TS:   s === [...s].reverse().join("")
来源：http://hek.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://fja.fzhhl.top

Go:   // 双指针从两端比较
来源：http://blz.zdbjq.cn

Ruby: s == s.reverse
来源：http://dmq.jinqigfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://luy.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://gwm.jinyuanbaomall.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://kjm.9152youxi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://aww.chenlongwang.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gtt.yj20258888.top

TS:   // 手写 Map<string, number>
来源：http://wbr.hysaishi.cn

Java: // 手写 HashMap
来源：http://bdk.wangdashe.top


<!-- 参考信息 -->