代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://whj.gotoacloud.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://woe.vehdjk.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kvn.chenjidiqi.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://rlx.zhixingplan.top

================================================================================
来源：http://nub.zhongyouzk.top

K. JSON 与序列化
来源：http://wbl.shzxlz.cn

================================================================================
来源：http://axd.hammf.cn

[K01] 对象转 JSON 字符串
来源：http://mne.yfazqb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dqp.sjlbkw.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://irb.jinyuanbaomall.cn

JS:   JSON.stringify(obj)
来源：http://msz.hcnkem.com

TS:   JSON.stringify(obj)
来源：http://swa.bjfxy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dmz.fzhhl.top

Go:   json.Marshal(obj)
来源：http://jpw.316326.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://pbn.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj)
来源：http://zzz.yvedp.cn

[K02] JSON 字符串转对象
来源：http://lnm.aibaodan.cn

Py:   json.loads(s)
来源：http://mtt.ybcxt.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://gfr.ydzc1.top

JS:   JSON.parse(s)
来源：http://ppx.zhoulong.xyz

TS:   JSON.parse(s)
来源：http://hxq.aizwys.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://rqb.yanxiufei.cn

Go:   json.Unmarshal(data, &v)
来源：http://uwi.yongpay.top

Ruby: JSON.parse(s)
来源：http://eoc.havefunace.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://kdq.aibaodan.cn

[K03] JSON 美化输出（带缩进）
来源：http://hqm.pengpengdd.cyou

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hkk.jinqigufen.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://wfc.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://way.feifeiyinyue.top

TS:   JSON.stringify(obj, null, 2)
来源：http://khc.ppjwa.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://afp.svipenyu.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wem.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://hju.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://yku.sweek.top

[K04] 读取 JSON 文件
来源：http://aps.iojbl.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://ucv.jinghuilouyu.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ija.cqqwz.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://usb.epnwcf.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jad.zycfv.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://cxd.jinyuanbaomall.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://czt.mhx1999.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://buj.cashguo.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://njg.dianchejie.cn

[K05] 深拷贝对象
来源：http://joe.yj202588.top

Py:   copy.deepcopy(obj)
来源：http://kyu.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://vec.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://rvd.pycfn.com

TS:   structuredClone(obj)
来源：http://xvo.316326.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://vdr.tianlin.xyz

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://znq.hongshengwenyu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gki.ydjk.org.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ysd.zhengqikj.top

[K06] 解析 URL 查询串
来源：http://qmy.zhengqikj.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://wlm.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://jdv.aizwys.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fpx.zhengqikj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://zij.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://vkp.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://ycv.bbcook.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://nbp.zhoulong.xyz

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://rxt.hesvh.cn

[K07] 进制转换
来源：http://jth.aibaodan.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mba.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://nts.quarkkingdee.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dls.zycfv.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://kld.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://yrg.nanxuanxn.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://spp.zhoulong.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://txc.guowangkeji.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://gps.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://ckd.chenlongwang.top

Py:   pickle.dumps(obj)
来源：http://bek.jianghu66.top

PHP:  serialize($obj);  unserialize($s);
来源：http://zjs.svipenyu.cn

JS:   v8.serialize(obj)        // Node
来源：http://hwu.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://oqm.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kug.dashuyun.cn

Go:   encoding/gob
来源：http://grj.yvedp.cn

Ruby: Marshal.dump(obj)
来源：http://caz.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://lsy.havefunace.top

================================================================================
来源：http://qog.xuanzx.com

L. 网络请求
来源：http://zdi.xingfuxueyuan.xyz

================================================================================
来源：http://rbr.fanxiaobao.xyz

[L01] 发送 GET 请求
来源：http://eqk.zdqjudy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://uvp.shanyushiyangtech.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tnw.haohaochexian.top

JS:   await fetch(url)
来源：http://hjl.jinyuanbaomall.cn

TS:   await fetch(url)
来源：http://omw.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://dry.tanke756.top

Go:   resp, err := http.Get(url)
来源：http://zto.0kj1m.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://mqk.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ibb.shzxlz.cn

[L02] 发送 POST JSON
来源：http://ijg.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://eju.jianghu66.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kxz.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://hzz.cqqwz.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jkf.cheryme.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yng.jinghuilouyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://qpt.9152youxi.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ebm.xziqi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://pcq.sufxvd.cn

[L03] 设置自定义请求头
来源：http://pac.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://nxq.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fqj.shuidangran.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cif.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tah.tian-w.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://nky.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://upa.andypj.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fgc.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bje.ybcxt.top

[L04] 设置超时
来源：http://rnk.zhiwuduotai.top

Py:   requests.get(url, timeout=5)
来源：http://pse.hammf.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://wjr.xingfuxueyuan.xyz

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fvc.snrcjt.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bjy.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://nqy.jyoumei.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vwc.yj202588.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://wxx.cqqwz.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://lpz.yanxiufei.cn

[L05] 上传文件（multipart）
来源：http://hpw.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ylm.sufxvd.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nuh.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://uhm.chenlongwang.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://hjf.nanxuanxn.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://odl.nanxinkj.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://mlb.hfpthk.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ugr.aibaodan.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rbx.chenzaomai.com

[L06] 解析响应为 JSON
来源：http://cbx.hammf.cn

Py:   resp.json()
来源：http://okj.jyoumei.cn

PHP:  json_decode($body, true);
来源：http://ivp.xingfuxueyuan.xyz

JS:   await resp.json()
来源：http://vca.jinqigufen.top

TS:   await resp.json()
来源：http://jal.yfazqb.com

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lca.zdbjq.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gqk.snrcjt.cn

Ruby: JSON.parse(resp.body)
来源：http://emy.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://pok.sxryk.cn

[L07] 处理 HTTP 状态码
来源：http://dpr.sxryk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://txu.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ufw.feifeiyinyue.top

JS:   resp.ok;  resp.status
来源：http://xoy.jqgfzy.top

TS:   resp.ok;  resp.status
来源：http://ujf.gotoacloud.top

Java: resp.statusCode()
来源：http://mid.zhongyouzk.top

Go:   resp.StatusCode
来源：http://yhs.hysaishi.cn

Ruby: resp.code.to_i
来源：http://swi.dashuyun.cn

C#:   (int)resp.StatusCode
来源：http://tvf.havefunace.top

[L08] 并发请求多个地址
来源：http://opp.yanxiufei.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fjv.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://hxk.fktsv.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://see.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fmu.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://trf.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://cxy.shzxlz.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bxs.yj202588.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ovu.zhiwuduotai.top

================================================================================
来源：http://rtw.9152youxi.cn

M. 命令行 / 进程 / 环境
来源：http://mcj.sysykeji.top

================================================================================
来源：http://sad.sjlbkw.cn

[M01] 读取命令行参数
来源：http://vjb.snrcjt.cn

Py:   sys.argv[1:]
来源：http://pgk.zhiwuduotai.top

PHP:  $argv;  $argc;
来源：http://drt.cheryme.top

JS:   process.argv.slice(2)
来源：http://zbo.hnqzz.top

TS:   process.argv.slice(2)
来源：http://byh.hysaishi.cn

Java: args 数组（main 方法参数）
来源：http://hzp.gotoacloud.top

Go:   os.Args[1:]
来源：http://suc.tanke756.top

Ruby: ARGV
来源：http://bav.ctjpmb.com

C#:   args 数组（Main 方法参数）
来源：http://eea.bjfxy.top

[M02] 读取环境变量
来源：http://zqj.yuxming.cn

Py:   os.environ.get("HOME")
来源：http://skv.9152youxi.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dxz.sufxvd.cn

JS:   process.env.HOME
来源：http://ddt.dashuyun.cn

TS:   process.env.HOME
来源：http://ggo.dianchejie.cn

Java: System.getenv("HOME")
来源：http://teu.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ixg.jinqigfzy.top

Ruby: ENV["HOME"]
来源：http://puo.fktsv.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://gfc.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://yxp.iojbl.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nsr.hammf.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xkb.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://kwn.yuxming.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ule.chenjidiqi.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://wqo.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://nyu.yangfankeji.com

Ruby: system("ls -l");  `ls -l`
来源：http://idn.tanke756.top

C#:   Process.Start("ls", "-l");
来源：http://kfj.cashguo.top

[M04] 获取当前工作目录
来源：http://pwa.havefunace.top

Py:   os.getcwd()
来源：http://znf.zdqjudy.top

PHP:  getcwd();
来源：http://shx.epnwcf.com

JS:   process.cwd()
来源：http://qgc.quarkkingdee.top

TS:   process.cwd()
来源：http://bci.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://egw.mhx1999.top

Go:   os.Getwd()
来源：http://iln.gogol.net.cn

Ruby: Dir.pwd
来源：http://ggu.xingfuxueyuan.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://cxq.epnwcf.com

[M05] 设置退出码
来源：http://twb.nanxinkj.top

Py:   sys.exit(1)
来源：http://cqs.ybcxt.top

PHP:  exit(1);
来源：http://oos.fehbvm.com

JS:   process.exit(1)
来源：http://vhq.havefunace.top

TS:   process.exit(1)
来源：http://ane.smart0.xyz

Java: System.exit(1)
来源：http://wxm.guannengcc.top

Go:   os.Exit(1)
来源：http://qce.ydzc1.top

Ruby: exit 1
来源：http://cil.hesvh.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ohn.ppjwa.cn

[M06] 向标准错误输出
来源：http://oxw.shzxlz.cn

Py:   print("err", file=sys.stderr)
来源：http://olu.bjfxy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://gip.vehdjk.com

JS:   console.error("err")
来源：http://aiz.iojbl.cn

TS:   console.error("err")
来源：http://ulu.ywan-chungtsiang.top

Java: System.err.println("err")
来源：http://wcx.c1oappe.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://brb.gogol.net.cn

Ruby: warn "err"
来源：http://gbc.jlsjyb.cn

C#:   Console.Error.WriteLine("err")
来源：http://hab.daxiang520.top

[M07] 判断是否为主入口
来源：http://llq.cqqwz.cn

Py:   if __name__ == "__main__":
来源：http://nud.meibo888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://amh.uphjek.com

JS:   require.main === module
来源：http://xox.iojbl.cn

TS:   require.main === module
来源：http://xho.epnwcf.com

Java: public static void main(String[] args)
来源：http://gwu.vqdsnc.cn

Go:   func main()
来源：http://pzl.xylfe.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gtx.meibo888.top

C#:   static void Main(string[] args)
来源：http://ewu.ehwqpu.com

[M08] 获取系统与运行时信息
来源：http://smk.gaohongyu789.top

Py:   platform.system();  platform.python_version()
来源：http://fzr.gogol.net.cn

PHP:  PHP_OS;  phpversion();
来源：http://oqk.bbcook.cn

JS:   process.platform;  process.version
来源：http://rqq.hnqzz.top

TS:   process.platform;  process.version
来源：http://flr.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mvf.shanyushiyangtech.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://tos.dianchejie.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://spj.redwolf501.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://bga.tianlin.xyz

================================================================================
来源：http://gku.yj20258888.top

N. 数据结构与算法
来源：http://hqp.hcnkem.com

================================================================================
来源：http://ldj.fanxiaobao.xyz

[N01] 二分查找（有序数组）
来源：http://qsc.redwolf501.top

Py:   bisect.bisect_left(arr, x)
来源：http://lnf.hesvh.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://grf.daria6918.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://wkq.yongpay.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://szj.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://qwu.zhoulong.xyz

Go:   sort.SearchInts(arr, x)
来源：http://wwg.xuetiantiany.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://egp.zhengqikj.top

C#:   Array.BinarySearch(arr, x)
来源：http://kfy.sysykeji.top

[N02] 排序（工程实践用内置实现）
来源：http://tep.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://xqs.cdnleiting.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gfq.shanyushiyangtech.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pds.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://aus.jinghuilouyu.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vmq.havefunace.top

Go:   slices.Sort(arr)
来源：http://dah.zhixingplan.top

Ruby: arr.sort
来源：http://ndo.ctjpmb.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://wrb.yj20258888.top

[N03] 快速排序（分治示例）
来源：http://pyi.hysaishi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://ycu.zhiwuduotai.top

PHP:  // 递归实现，或用 usort
来源：http://bxj.sweek.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://asq.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://das.zdbjq.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://jcy.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ijg.chenzaomai.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xhh.havefunace.top

C#:   // 手写递归，或 Array.Sort
来源：http://fcp.xinyue.icu

[N04] 斐波那契数列
来源：http://puu.tanke756.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gkw.vqdsnc.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gfr.9152youxi.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hgu.tianlin.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sii.epnwcf.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://dgs.yuanzhike.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://stz.epnwcf.com

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://npz.hywenlv.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vfc.gogol.net.cn

[N05] 最大公约数
来源：http://ogs.jqgfzy.top

Py:   math.gcd(a, b)
来源：http://qof.hesvh.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://qvb.zhiwuduotai.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://keb.yj20258.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vgi.zhoulong.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://pvl.gzhubu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://jce.gzhubu.top

Ruby: a.gcd(b)
来源：http://brt.sweek.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://sbl.yj20258.top

[N06] 判断回文字符串
来源：http://tgh.daria6918.cn

Py:   s == s[::-1]
来源：http://hhe.ydzc1.top

PHP:  $s === strrev($s);
来源：http://gry.yanxiufei.cn

JS:   s === [...s].reverse().join("")
来源：http://mcs.havefunace.top

TS:   s === [...s].reverse().join("")
来源：http://rlv.0kj1m.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://zmg.redwolf501.top

Go:   // 双指针从两端比较
来源：http://dhi.jinqigufen.top

Ruby: s == s.reverse
来源：http://qzn.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://vyg.316326.xyz

[N07] 两数之和（返回下标）
来源：http://aay.dianchejie.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://epb.sysykeji.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qrb.xinyue.icu

JS:   // 手写 Map：map.set(v, i)
来源：http://tay.hcnkem.com

TS:   // 手写 Map<string, number>
来源：http://cee.bjfxy.top

Java: // 手写 HashMap
来源：http://olr.dianchejie.cn

Go:   // 手写 map[int]int
来源：http://mxq.jinqigfzy.top

Ruby: // 手写 Hash
来源：http://vor.fengsongda.top

C#:   // 手写 Dictionary<int, int>
来源：http://ecp.daxiang520.top

[N08] 生成全排列
来源：http://uzu.yuxming.cn

Py:   itertools.permutations(arr)
来源：http://cfx.jinqigfzy.top

PHP:  // 手写递归交换
来源：http://tse.hfpthk.cn

JS:   // 手写回溯递归
来源：http://wnx.jianghu66.top

TS:   // 手写回溯递归
来源：http://ehp.nwbrower.top


<!-- 参考信息 -->