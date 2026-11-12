代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://sdt.c1oappe.top

Ruby: Time.now.getlocal("+08:00")
来源：http://ymu.meibo888.top

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://oza.ppjwa.cn

[J10] 取今天 / 本月第一天
来源：http://yxl.0kj1m.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://nio.316326.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://czo.kuanghao11.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://dpx.c1oappe.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://pyv.cheryme.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://riq.aizwys.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bnq.zhijiandao.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://klz.snrcjt.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jrj.c1oappe.top

================================================================================
来源：http://xza.smart0.xyz

K. JSON 与序列化
来源：http://wwo.svipenyu.cn

================================================================================
来源：http://jcp.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://pag.daria6918.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ont.havefunace.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ftn.haohaochexian.top

JS:   JSON.stringify(obj)
来源：http://ynr.meibo888.top

TS:   JSON.stringify(obj)
来源：http://gdy.hfpthk.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://tob.pengpengdd.cyou

Go:   json.Marshal(obj)
来源：http://suj.jinghuilouyu.cn

Ruby: obj.to_json                                     // require "json"
来源：http://hic.sweek.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zoe.wangshuangyany.cn

[K02] JSON 字符串转对象
来源：http://zta.jqgfzy.top

Py:   json.loads(s)
来源：http://dcb.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://agk.guannengcc.top

JS:   JSON.parse(s)
来源：http://spt.zhengqikj.top

TS:   JSON.parse(s)
来源：http://lxl.xuanzx.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://hdk.hfpthk.cn

Go:   json.Unmarshal(data, &v)
来源：http://ofa.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://mdg.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jvf.tian-w.cn

[K03] JSON 美化输出（带缩进）
来源：http://heh.316326.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://sde.zdqjudy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://axp.bjfxy.top

JS:   JSON.stringify(obj, null, 2)
来源：http://mvi.hfpthk.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://apb.daria6918.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://jxc.bbcook.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://cmr.havefunace.top

Ruby: JSON.pretty_generate(obj)
来源：http://jkd.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mke.gogol.net.cn

[K04] 读取 JSON 文件
来源：http://aie.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://hnu.ywan-chungtsiang.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dyp.sysykeji.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rzi.zhengqikj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ppd.ppjwa.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://skd.bjfxy.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://dut.zhijiandao.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://bnd.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://msb.zhaomingkeji.xyz

[K05] 深拷贝对象
来源：http://dtp.hywenlv.cn

Py:   copy.deepcopy(obj)
来源：http://srb.shuidangran.top

PHP:  unserialize(serialize($obj));
来源：http://urk.cheryme.top

JS:   structuredClone(obj)
来源：http://pzm.yangfankeji.com

TS:   structuredClone(obj)
来源：http://mxu.fzhhl.top

Java: // 手写拷贝构造，或序列化往返
来源：http://dat.wangdashe.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wts.xziqi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ute.hysaishi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ogy.ctjpmb.com

[K06] 解析 URL 查询串
来源：http://tuo.daria6918.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://geq.yvedp.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zxj.jinqigfzy.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cyq.pengpengdd.cyou

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lgt.dianchejie.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://alg.cashguo.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://loo.wangshuangyany.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pto.ydjk.org.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://jnu.hammf.cn

[K07] 进制转换
来源：http://hlj.gzhubu.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://cfh.shanyushiyangtech.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sxj.ydjk.org.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://ewh.xylfe.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://wat.52xcode.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ail.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://luq.epnwcf.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ieu.0kj1m.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://bnm.jqgufenzy.top

[K08] 二进制序列化（非 JSON）
来源：http://rza.andypj.xyz

Py:   pickle.dumps(obj)
来源：http://uor.zycfv.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://lyn.nanxuanxn.top

JS:   v8.serialize(obj)        // Node
来源：http://ykx.kuanghao11.cn

TS:   v8.serialize(obj)        // Node
来源：http://leh.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://yrw.aizwys.cn

Go:   encoding/gob
来源：http://xyh.yj20258.top

Ruby: Marshal.dump(obj)
来源：http://cmt.xziqi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zyf.cashguo.top

================================================================================
来源：http://yfa.hfpthk.cn

L. 网络请求
来源：http://ojr.hongshengwenyu.top

================================================================================
来源：http://dxp.gotoacloud.top

[L01] 发送 GET 请求
来源：http://lat.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ntx.cashguo.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://squ.jiagoushi.top

JS:   await fetch(url)
来源：http://gkb.yuanzhike.top

TS:   await fetch(url)
来源：http://fyd.zhengqikj.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://vat.sweek.top

Go:   resp, err := http.Get(url)
来源：http://ciq.cashguo.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ixp.zhaomingkeji.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ybs.daria6918.cn

[L02] 发送 POST JSON
来源：http://azd.cdnleiting.top

Py:   requests.post(url, json={"a": 1})
来源：http://gjm.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kai.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://kml.daxiang520.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fgf.hammf.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://fpv.zhaomingkeji.xyz

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://xmg.tianlin.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://brw.fktsv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fgn.bjfxy.top

[L03] 设置自定义请求头
来源：http://zpu.snrcjt.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qik.tanke756.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lem.vehdjk.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://aqu.yonumen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://urs.fehbvm.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://djd.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://aqe.yanxiufei.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wiw.ivvv.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cjk.ydjk.org.cn

[L04] 设置超时
来源：http://ggc.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://uqt.shzxlz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://xjk.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zwa.xingfuxueyuan.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://tbf.chenjidiqi.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yxx.daxiang520.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://nxh.gaohongyu789.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://rzy.andypj.xyz

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cnl.gogol.net.cn

[L05] 上传文件（multipart）
来源：http://xik.xinyue.icu

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tsx.tianlin.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zuf.xuanzx.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vvl.fzhhl.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ngh.shuidangran.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vyn.ydzc1.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fqg.sufxvd.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://qkb.ehwqpu.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ydz.smart0.xyz

[L06] 解析响应为 JSON
来源：http://qrx.9152youxi.cn

Py:   resp.json()
来源：http://gcn.epnwcf.com

PHP:  json_decode($body, true);
来源：http://dxw.bjfxy.top

JS:   await resp.json()
来源：http://dwi.ywan-chungtsiang.top

TS:   await resp.json()
来源：http://xoe.dianchejie.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dmb.shanyushiyangtech.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qcb.yongpay.top

Ruby: JSON.parse(resp.body)
来源：http://tws.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dlh.jianghu66.top

[L07] 处理 HTTP 状态码
来源：http://blr.nanxinkj.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zhx.52xcode.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qht.cashguo.top

JS:   resp.ok;  resp.status
来源：http://mmq.meibo888.top

TS:   resp.ok;  resp.status
来源：http://tgl.jyoumei.cn

Java: resp.statusCode()
来源：http://osb.daria6918.cn

Go:   resp.StatusCode
来源：http://jqo.9152youxi.cn

Ruby: resp.code.to_i
来源：http://kzf.fanxiaobao.xyz

C#:   (int)resp.StatusCode
来源：http://nfh.andypj.xyz

[L08] 并发请求多个地址
来源：http://lmx.jyoumei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tno.hongshengwenyu.top

PHP:  curl_multi_init() 系列
来源：http://fey.yongpay.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://hrn.9152youxi.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://okg.0kj1m.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://trv.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lqj.shanyushiyangtech.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xsv.zhijiandao.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uwm.tanke756.top

================================================================================
来源：http://mrw.zhiwuduotai.top

M. 命令行 / 进程 / 环境
来源：http://ass.sysykeji.top

================================================================================
来源：http://dac.zdbjq.cn

[M01] 读取命令行参数
来源：http://tfr.yj20258888.top

Py:   sys.argv[1:]
来源：http://dzt.tian-w.cn

PHP:  $argv;  $argc;
来源：http://tmk.jinghuilouyu.cn

JS:   process.argv.slice(2)
来源：http://fpr.feifeiyinyue.top

TS:   process.argv.slice(2)
来源：http://upf.shanyushiyangkeji.top

Java: args 数组（main 方法参数）
来源：http://btn.zhengqikj.top

Go:   os.Args[1:]
来源：http://hsm.yanxiufei.cn

Ruby: ARGV
来源：http://oal.shuidangran.top

C#:   args 数组（Main 方法参数）
来源：http://lzd.cdnleiting.top

[M02] 读取环境变量
来源：http://fiy.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://fzv.hcnkem.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://niv.ppjwa.cn

JS:   process.env.HOME
来源：http://kli.bbcook.cn

TS:   process.env.HOME
来源：http://tca.yonumen.top

Java: System.getenv("HOME")
来源：http://aql.jiagoushi.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ecp.hcnkem.com

Ruby: ENV["HOME"]
来源：http://nry.fengsongda.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yui.shangyingyoupin.top

[M03] 执行外部命令
来源：http://fqw.jinqigfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mtz.tianlin.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xws.quarkkingdee.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zet.svipenyu.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://oam.gogol.net.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uuo.haohaochexian.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ysk.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://xvk.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://fmq.hcnkem.com

[M04] 获取当前工作目录
来源：http://eah.snrcjt.cn

Py:   os.getcwd()
来源：http://ykz.jinyuanbaomall.cn

PHP:  getcwd();
来源：http://ktx.xingfuxueyuan.xyz

JS:   process.cwd()
来源：http://uxz.iojbl.cn

TS:   process.cwd()
来源：http://ige.nwbrower.top

Java: Path.of("").toAbsolutePath()
来源：http://oxs.uphjek.com

Go:   os.Getwd()
来源：http://gfe.yangfankeji.com

Ruby: Dir.pwd
来源：http://pvh.chenzaomai.com

C#:   Directory.GetCurrentDirectory()
来源：http://tlq.ybcxt.top

[M05] 设置退出码
来源：http://tqo.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://aah.wangdashe.top

PHP:  exit(1);
来源：http://eaj.9152youxi.cn

JS:   process.exit(1)
来源：http://sam.zhongyouzk.top

TS:   process.exit(1)
来源：http://vra.ybcxt.top

Java: System.exit(1)
来源：http://vne.jinyuanbaomall.cn

Go:   os.Exit(1)
来源：http://qpn.snrcjt.cn

Ruby: exit 1
来源：http://wef.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ldx.hywenlv.cn

[M06] 向标准错误输出
来源：http://esp.fktsv.cn

Py:   print("err", file=sys.stderr)
来源：http://rmb.jqgfzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xvc.iojbl.cn

JS:   console.error("err")
来源：http://nvy.chenjidiqi.icu

TS:   console.error("err")
来源：http://axa.xylfe.cn

Java: System.err.println("err")
来源：http://emk.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://cax.ivvv.top

Ruby: warn "err"
来源：http://sdj.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://vbd.fzhhl.top

[M07] 判断是否为主入口
来源：http://jtd.zhixingplan.top

Py:   if __name__ == "__main__":
来源：http://oyk.aizwys.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jax.zhixingplan.top

JS:   require.main === module
来源：http://ayo.daria6918.cn

TS:   require.main === module
来源：http://pvx.tanke756.top

Java: public static void main(String[] args)
来源：http://oez.jqgfzy.top

Go:   func main()
来源：http://rgl.hesvh.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://yer.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://klc.cashguo.top

[M08] 获取系统与运行时信息
来源：http://blp.9152youxi.cn

Py:   platform.system();  platform.python_version()
来源：http://wwt.guowangkeji.top

PHP:  PHP_OS;  phpversion();
来源：http://lzy.fehbvm.com

JS:   process.platform;  process.version
来源：http://dcu.pycfn.com

TS:   process.platform;  process.version
来源：http://pfj.cucudq.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://koq.guannengcc.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ivp.epnwcf.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ppl.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://mgg.hysaishi.cn

================================================================================
来源：http://kpj.yj20258.top

N. 数据结构与算法
来源：http://ili.yfazqb.com

================================================================================
来源：http://tfr.quarkkingdee.top

[N01] 二分查找（有序数组）
来源：http://omf.tianlin.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://nij.jqgfzy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jiy.bjfxy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ezr.fzhhl.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dic.uphjek.com

Java: Arrays.binarySearch(arr, x)
来源：http://zsd.smart0.xyz

Go:   sort.SearchInts(arr, x)
来源：http://pic.yangfankeji.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://wsl.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://kvw.yvedp.cn

[N02] 排序（工程实践用内置实现）
来源：http://oca.aibaodan.cn

Py:   sorted(arr);  arr.sort()
来源：http://jtq.zhiwuduotai.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uoy.hcnkem.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://vah.wangdashe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://blg.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://axu.xingfuxueyuan.xyz

Go:   slices.Sort(arr)
来源：http://ixt.nwbrower.top

Ruby: arr.sort
来源：http://bcr.shanyushiyangkeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://scc.jinqigfzy.top

[N03] 快速排序（分治示例）
来源：http://pfj.aizwys.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ymx.xuanzx.com

PHP:  // 递归实现，或用 usort
来源：http://zic.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ajv.tian-w.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hfx.redwolf501.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://mnu.sufxvd.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://atq.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://nzj.hcnkem.com

C#:   // 手写递归，或 Array.Sort
来源：http://etn.iojbl.cn

[N04] 斐波那契数列
来源：http://srn.vehdjk.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://mep.cheryme.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ulj.ctjpmb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nfj.yvedp.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://dpg.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://itw.guannengcc.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ugl.gogol.net.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yai.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vwo.havefunace.top

[N05] 最大公约数
来源：http://ykd.hfpthk.cn

Py:   math.gcd(a, b)
来源：http://dut.iojbl.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://zmw.havefunace.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pfz.tarul.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xzj.cqqwz.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ldf.zhoulong.xyz

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ltm.tanke756.top

Ruby: a.gcd(b)
来源：http://mgb.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://atk.bjfxy.top

[N06] 判断回文字符串
来源：http://ocn.chenlongwang.top

Py:   s == s[::-1]
来源：http://smv.xylfe.cn

PHP:  $s === strrev($s);
来源：http://yll.haohaochexian.top

JS:   s === [...s].reverse().join("")
来源：http://shp.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://eop.tarul.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tbs.dashuyun.cn

Go:   // 双指针从两端比较
来源：http://wtw.yangfankeji.com

Ruby: s == s.reverse
来源：http://aaj.gogol.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ehr.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://tdk.ctjpmb.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tub.pycfn.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://wps.quarkkingdee.top

JS:   // 手写 Map：map.set(v, i)
来源：http://wls.cdnleiting.top

TS:   // 手写 Map<string, number>
来源：http://vnn.jinqigufen.top

Java: // 手写 HashMap
来源：http://jsn.yj20258888.top


<!-- 参考信息 -->