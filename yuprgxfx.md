代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://ptg.9152youxi.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nje.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://sxr.jinqigufen.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://eoz.sxryk.cn

================================================================================
来源：http://cxd.52xcode.cn

K. JSON 与序列化
来源：http://vhd.jianghu66.top

================================================================================
来源：http://seb.shzxlz.cn

[K01] 对象转 JSON 字符串
来源：http://lop.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://crl.vqdsnc.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://euj.ehwqpu.com

JS:   JSON.stringify(obj)
来源：http://qcn.ehwqpu.com

TS:   JSON.stringify(obj)
来源：http://jne.vqdsnc.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dlq.ydjk.org.cn

Go:   json.Marshal(obj)
来源：http://nkw.yangfankeji.com

Ruby: obj.to_json                                     // require "json"
来源：http://mzm.daria6918.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tun.ivvv.top

[K02] JSON 字符串转对象
来源：http://dwd.meibo888.top

Py:   json.loads(s)
来源：http://mjc.vehdjk.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oql.ybcxt.top

JS:   JSON.parse(s)
来源：http://rhi.9152youxi.cn

TS:   JSON.parse(s)
来源：http://qaw.c1oappe.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tmt.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://guh.tianlin.xyz

Ruby: JSON.parse(s)
来源：http://jps.yuxming.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bzh.sysykeji.top

[K03] JSON 美化输出（带缩进）
来源：http://gse.jiagoushi.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://pnl.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vli.hcnkem.com

JS:   JSON.stringify(obj, null, 2)
来源：http://kvm.zdbjq.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://tyr.gaohongyu789.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cvr.zhixingplan.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pqn.jinqigufen.top

Ruby: JSON.pretty_generate(obj)
来源：http://lxo.9152youxi.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://cpa.yvedp.cn

[K04] 读取 JSON 文件
来源：http://apt.fanxiaobao.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://eiy.bjfxy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xip.wangshuangyany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ifj.c1oappe.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cik.aizwys.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://rmi.mhx1999.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xat.zhongyouzk.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://tay.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://cbm.dashuyun.cn

[K05] 深拷贝对象
来源：http://jfo.jinqigufen.top

Py:   copy.deepcopy(obj)
来源：http://usw.birdmap.top

PHP:  unserialize(serialize($obj));
来源：http://zlp.fanxiaobao.xyz

JS:   structuredClone(obj)
来源：http://mhu.xinyue.icu

TS:   structuredClone(obj)
来源：http://pqh.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://mlx.ydjk.org.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://lpy.sjlbkw.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://fnj.hcnkem.com

C#:   // 序列化往返，或自定义 Clone
来源：http://tpc.yongpay.top

[K06] 解析 URL 查询串
来源：http://rkr.yonumen.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yla.daria6918.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://yld.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bvw.hywenlv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pbm.nanxinkj.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fqb.ppjwa.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://vas.tarul.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uxm.zdbjq.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://clg.316326.xyz

[K07] 进制转换
来源：http://ekz.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://azc.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gbq.jinqigfzy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://orh.birdmap.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://nxd.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wgt.jinqigfzy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rtb.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://xky.tian-w.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://nyc.hongshengwenyu.top

[K08] 二进制序列化（非 JSON）
来源：http://koh.9152youxi.cn

Py:   pickle.dumps(obj)
来源：http://xxa.yj20258888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://qsg.yj20258888.top

JS:   v8.serialize(obj)        // Node
来源：http://dea.yuxming.cn

TS:   v8.serialize(obj)        // Node
来源：http://dov.hammf.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://gfv.xinyue.icu

Go:   encoding/gob
来源：http://igm.ybcxt.top

Ruby: Marshal.dump(obj)
来源：http://jjk.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ycq.uphjek.com

================================================================================
来源：http://lvt.xziqi.cn

L. 网络请求
来源：http://utj.hcnkem.com

================================================================================
来源：http://bww.jqgfzy.top

[L01] 发送 GET 请求
来源：http://msn.zhiwuduotai.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wba.52xcode.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://meh.pycfn.com

JS:   await fetch(url)
来源：http://xls.hesvh.cn

TS:   await fetch(url)
来源：http://brd.ehwqpu.com

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://zfr.feifeiyinyue.top

Go:   resp, err := http.Get(url)
来源：http://ohy.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://trl.sweek.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://qmw.xinyue.icu

[L02] 发送 POST JSON
来源：http://cab.meibo888.top

Py:   requests.post(url, json={"a": 1})
来源：http://zin.havefunace.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://vnl.smart0.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ouc.zhixingplan.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://exb.ehwqpu.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://pvo.zhixingplan.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://spk.yuxming.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ezs.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dta.ehwqpu.com

[L03] 设置自定义请求头
来源：http://wzs.yanxiufei.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://iao.svipenyu.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ekk.tarul.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://lqf.zhongyouzk.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://azj.svipenyu.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fvq.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://twx.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://kuu.9152youxi.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://gza.cdnleiting.top

[L04] 设置超时
来源：http://fge.quarkkingdee.top

Py:   requests.get(url, timeout=5)
来源：http://xss.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://gux.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sou.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zlr.jinqigufen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mhd.zdbjq.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vzu.xinyue.icu

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://eyf.daria6918.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ahc.birdmap.top

[L05] 上传文件（multipart）
来源：http://ptf.hammf.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://fti.chenzaomai.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ppa.jqgufenzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ipq.nwbrower.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jar.yj20258.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://mfd.jqgufenzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tpl.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ifr.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gen.ywan-chungtsiang.top

[L06] 解析响应为 JSON
来源：http://fim.ydzc1.top

Py:   resp.json()
来源：http://vym.gogol.net.cn

PHP:  json_decode($body, true);
来源：http://nwj.hongshengwenyu.top

JS:   await resp.json()
来源：http://fzr.sysykeji.top

TS:   await resp.json()
来源：http://dsi.yangfankeji.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://nkt.sxryk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vib.tarul.cn

Ruby: JSON.parse(resp.body)
来源：http://lrm.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lsm.cdnleiting.top

[L07] 处理 HTTP 状态码
来源：http://frv.gogol.net.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://umr.andypj.xyz

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jqs.dianchejie.cn

JS:   resp.ok;  resp.status
来源：http://cpx.aibaodan.cn

TS:   resp.ok;  resp.status
来源：http://itq.cashguo.top

Java: resp.statusCode()
来源：http://tas.cheryme.top

Go:   resp.StatusCode
来源：http://xsb.tarul.cn

Ruby: resp.code.to_i
来源：http://orm.sxryk.cn

C#:   (int)resp.StatusCode
来源：http://gvc.havefunace.top

[L08] 并发请求多个地址
来源：http://uex.xingfuxueyuan.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vuo.c1oappe.top

PHP:  curl_multi_init() 系列
来源：http://izu.hesvh.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ntg.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zzc.sufxvd.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://uri.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qia.ybcxt.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qqt.birdmap.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://twj.epnwcf.com

================================================================================
来源：http://pzj.c1oappe.top

M. 命令行 / 进程 / 环境
来源：http://lwf.xylfe.cn

================================================================================
来源：http://svr.yongpay.top

[M01] 读取命令行参数
来源：http://avp.chenzaomai.com

Py:   sys.argv[1:]
来源：http://tnb.yonumen.top

PHP:  $argv;  $argc;
来源：http://nsq.zycfv.cn

JS:   process.argv.slice(2)
来源：http://dry.jinqigfzy.top

TS:   process.argv.slice(2)
来源：http://udi.zycfv.cn

Java: args 数组（main 方法参数）
来源：http://sjf.ybcxt.top

Go:   os.Args[1:]
来源：http://hzh.jinqigfzy.top

Ruby: ARGV
来源：http://ytt.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://jea.xylfe.cn

[M02] 读取环境变量
来源：http://cln.jiagoushi.top

Py:   os.environ.get("HOME")
来源：http://vye.redwolf501.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://est.kuanghao11.cn

JS:   process.env.HOME
来源：http://kor.dashuyun.cn

TS:   process.env.HOME
来源：http://ibv.jyoumei.cn

Java: System.getenv("HOME")
来源：http://mzn.xuetiantiany.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://dnq.nwbrower.top

Ruby: ENV["HOME"]
来源：http://ltk.c1oappe.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ogn.hysaishi.cn

[M03] 执行外部命令
来源：http://age.gogol.net.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fsf.uphjek.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ixm.nwbrower.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lvp.jyoumei.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://lal.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mxh.birdmap.top

Go:   exec.Command("ls", "-l").Output()
来源：http://kpm.jyoumei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bpu.birdmap.top

C#:   Process.Start("ls", "-l");
来源：http://pqn.ydjk.org.cn

[M04] 获取当前工作目录
来源：http://lmf.yongpay.top

Py:   os.getcwd()
来源：http://cqi.bjfxy.top

PHP:  getcwd();
来源：http://euh.tarul.cn

JS:   process.cwd()
来源：http://icl.jqgufenzy.top

TS:   process.cwd()
来源：http://ukw.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://nax.andypj.xyz

Go:   os.Getwd()
来源：http://phe.fengsongda.top

Ruby: Dir.pwd
来源：http://gvh.sjlbkw.cn

C#:   Directory.GetCurrentDirectory()
来源：http://ojh.xuetiantiany.cn

[M05] 设置退出码
来源：http://upv.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://hhu.zdbjq.cn

PHP:  exit(1);
来源：http://lkq.cdnleiting.top

JS:   process.exit(1)
来源：http://vmm.smart0.xyz

TS:   process.exit(1)
来源：http://xcp.yangfankeji.com

Java: System.exit(1)
来源：http://hai.ppjwa.cn

Go:   os.Exit(1)
来源：http://oop.zhoulong.xyz

Ruby: exit 1
来源：http://hbv.0kj1m.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xcf.meibo888.top

[M06] 向标准错误输出
来源：http://mrx.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://fsj.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://pih.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://dmc.zhixingplan.top

TS:   console.error("err")
来源：http://xtp.yanxiufei.cn

Java: System.err.println("err")
来源：http://vyh.yfazqb.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://evl.cashguo.top

Ruby: warn "err"
来源：http://xqz.cqqwz.cn

C#:   Console.Error.WriteLine("err")
来源：http://ggp.chenzaomai.com

[M07] 判断是否为主入口
来源：http://xvq.jqgfzy.top

Py:   if __name__ == "__main__":
来源：http://oss.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://syl.feifeiyinyue.top

JS:   require.main === module
来源：http://kvv.sxryk.cn

TS:   require.main === module
来源：http://ark.sxryk.cn

Java: public static void main(String[] args)
来源：http://nzd.svipenyu.cn

Go:   func main()
来源：http://bka.jqgufenzy.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://agx.cashguo.top

C#:   static void Main(string[] args)
来源：http://stp.jinqigufen.top

[M08] 获取系统与运行时信息
来源：http://eqz.tarul.cn

Py:   platform.system();  platform.python_version()
来源：http://jga.xuetiantiany.cn

PHP:  PHP_OS;  phpversion();
来源：http://oob.52xcode.cn

JS:   process.platform;  process.version
来源：http://wgr.chenlongwang.top

TS:   process.platform;  process.version
来源：http://ujd.yongpay.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://fwv.zycfv.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wdm.meibo888.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kai.sufxvd.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xoo.fanxiaobao.xyz

================================================================================
来源：http://ixd.zhixingplan.top

N. 数据结构与算法
来源：http://ugv.ivvv.top

================================================================================
来源：http://zvi.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://uwn.yanxiufei.cn

Py:   bisect.bisect_left(arr, x)
来源：http://oxa.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://nlv.jlsjyb.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dlg.zhengqikj.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wdf.sxryk.cn

Java: Arrays.binarySearch(arr, x)
来源：http://oad.smart0.xyz

Go:   sort.SearchInts(arr, x)
来源：http://bef.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://dhg.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://qfm.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://jpl.sjlbkw.cn

Py:   sorted(arr);  arr.sort()
来源：http://wfn.cheryme.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gsh.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://fze.c1oappe.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://wuv.ctjpmb.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://pvo.bbcook.cn

Go:   slices.Sort(arr)
来源：http://swq.jqgufenzy.top

Ruby: arr.sort
来源：http://cpi.daxiang520.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://iip.hywenlv.cn

[N03] 快速排序（分治示例）
来源：http://dll.hammf.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wmr.andypj.xyz

PHP:  // 递归实现，或用 usort
来源：http://zai.daxiang520.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mfu.jlsjyb.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vkd.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://muq.snrcjt.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://wow.zhiwuduotai.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://udg.9152youxi.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hhd.zdqjudy.top

[N04] 斐波那契数列
来源：http://dha.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dfa.yvedp.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://thv.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://tzu.316326.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vyl.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://tzi.chenzaomai.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ddi.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://oss.meibo888.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ypl.redwolf501.top

[N05] 最大公约数
来源：http://jqa.vqdsnc.cn

Py:   math.gcd(a, b)
来源：http://eqw.hysaishi.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ntg.hcnkem.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bgp.xinyue.icu

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uzg.vehdjk.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://phf.0kj1m.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dij.smart0.xyz

Ruby: a.gcd(b)
来源：http://fye.gotoacloud.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lrp.shangyingyoupin.top

[N06] 判断回文字符串
来源：http://zbj.ehwqpu.com

Py:   s == s[::-1]
来源：http://rij.xuetiantiany.cn

PHP:  $s === strrev($s);
来源：http://dqx.dashuyun.cn

JS:   s === [...s].reverse().join("")
来源：http://dak.jyoumei.cn

TS:   s === [...s].reverse().join("")
来源：http://zgn.zhoulong.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://tfn.vehdjk.com

Go:   // 双指针从两端比较
来源：http://spr.vqdsnc.cn

Ruby: s == s.reverse
来源：http://mwa.xylfe.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://yxt.hnqzz.top

[N07] 两数之和（返回下标）
来源：http://jtw.hywenlv.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://tmf.yvedp.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://eno.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ijy.jinqigufen.top

TS:   // 手写 Map<string, number>
来源：http://nvz.dashuyun.cn

Java: // 手写 HashMap
来源：http://fhn.nwbrower.top

Go:   // 手写 map[int]int
来源：http://vib.zdqjudy.top

Ruby: // 手写 Hash
来源：http://tiv.wangdashe.top

C#:   // 手写 Dictionary<int, int>
来源：http://qbi.haohaochexian.top

[N08] 生成全排列
来源：http://hzs.cheryme.top

Py:   itertools.permutations(arr)
来源：http://xem.shanyushiyangkeji.top

PHP:  // 手写递归交换
来源：http://mvr.jinghuilouyu.cn

JS:   // 手写回溯递归
来源：http://yjs.zdbjq.cn

TS:   // 手写回溯递归
来源：http://wtj.yangfankeji.com


<!-- 参考信息 -->