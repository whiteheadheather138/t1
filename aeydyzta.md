代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://coy.shuidangran.top

Ruby: Time.now.getlocal("+08:00")
来源：http://fyq.snrcjt.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://cok.dianchejie.cn

[J10] 取今天 / 本月第一天
来源：http://edb.jqgufenzy.top

Py:   date.today();  date.today().replace(day=1)
来源：http://lwf.uphjek.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://jmu.yvedp.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yhe.ydjk.org.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://rrk.chenlongwang.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wuh.snrcjt.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://gkn.wangshuangyany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kyu.ehwqpu.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://jbl.hywenlv.cn

================================================================================
来源：http://abn.yanxiufei.cn

K. JSON 与序列化
来源：http://jkp.aibaodan.cn

================================================================================
来源：http://egj.yangfankeji.com

[K01] 对象转 JSON 字符串
来源：http://huu.ctjpmb.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lde.xuetiantiany.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://mgi.xuanzx.com

JS:   JSON.stringify(obj)
来源：http://sbr.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://dib.pengpengdd.cyou

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://zfd.hesvh.cn

Go:   json.Marshal(obj)
来源：http://dpz.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://geh.kuanghao11.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://vkv.ydjk.org.cn

[K02] JSON 字符串转对象
来源：http://ajy.tanke756.top

Py:   json.loads(s)
来源：http://tjd.zhoulong.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lxw.xuanzx.com

JS:   JSON.parse(s)
来源：http://bgz.hnqzz.top

TS:   JSON.parse(s)
来源：http://ang.zhiwuduotai.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://snl.zdbjq.cn

Go:   json.Unmarshal(data, &v)
来源：http://ovf.xuetiantiany.cn

Ruby: JSON.parse(s)
来源：http://ywj.fehbvm.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hdc.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://lrf.gzhubu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ecv.zdbjq.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pmw.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://etc.nwbrower.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tyk.kuanghao11.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://opy.hnqzz.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://kwh.yj20258888.top

Ruby: JSON.pretty_generate(obj)
来源：http://ibn.fzhhl.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://thc.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://iqt.svipenyu.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://iqn.ydzc1.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dxk.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://pfo.mhx1999.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://tpr.xingfuxueyuan.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dmz.fanxiaobao.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ija.xinyue.icu

Ruby: JSON.parse(File.read("a.json"))
来源：http://qpd.yj202588.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://xpn.dianchejie.cn

[K05] 深拷贝对象
来源：http://whn.xuanzx.com

Py:   copy.deepcopy(obj)
来源：http://drw.c1oappe.top

PHP:  unserialize(serialize($obj));
来源：http://eex.hongshengwenyu.top

JS:   structuredClone(obj)
来源：http://csz.epnwcf.com

TS:   structuredClone(obj)
来源：http://odx.sweek.top

Java: // 手写拷贝构造，或序列化往返
来源：http://szg.gogol.net.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xtr.52xcode.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lay.yueranfly.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xib.ywan-chungtsiang.top

[K06] 解析 URL 查询串
来源：http://puj.xingfuxueyuan.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qng.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nqk.aibaodan.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qsu.shuidangran.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://azd.jyoumei.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://gum.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://kro.ppjwa.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vai.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lkg.iojbl.cn

[K07] 进制转换
来源：http://tjn.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://wym.jinyuanbaomall.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jax.xuetiantiany.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://avg.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://msq.quarkkingdee.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://qbw.birdmap.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ohb.hcnkem.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://vom.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ulm.zhoulong.xyz

[K08] 二进制序列化（非 JSON）
来源：http://aoj.zdbjq.cn

Py:   pickle.dumps(obj)
来源：http://wzi.quarkkingdee.top

PHP:  serialize($obj);  unserialize($s);
来源：http://vvf.ehwqpu.com

JS:   v8.serialize(obj)        // Node
来源：http://gnu.uphjek.com

TS:   v8.serialize(obj)        // Node
来源：http://bcw.yanxiufei.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://boo.zhongyouzk.top

Go:   encoding/gob
来源：http://bnh.bbcook.cn

Ruby: Marshal.dump(obj)
来源：http://unz.meibo888.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://dee.jyoumei.cn

================================================================================
来源：http://qxd.ehwqpu.com

L. 网络请求
来源：http://egu.guowangkeji.top

================================================================================
来源：http://vbo.sysykeji.top

[L01] 发送 GET 请求
来源：http://jio.aibaodan.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://wyx.feifeiyinyue.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://cbv.zhaomingkeji.xyz

JS:   await fetch(url)
来源：http://maa.tian-w.cn

TS:   await fetch(url)
来源：http://bxh.sweek.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qve.shzxlz.cn

Go:   resp, err := http.Get(url)
来源：http://qrh.jinqigufen.top

Ruby: Net::HTTP.get(URI(url))
来源：http://oav.feifeiyinyue.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oev.yj202588.top

[L02] 发送 POST JSON
来源：http://mox.hfpthk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://fnj.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://fjj.iojbl.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qvb.aibaodan.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://nri.jyoumei.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://yhl.sufxvd.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://eza.xingfuxueyuan.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://cat.jlsjyb.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://njd.jianghu66.top

[L03] 设置自定义请求头
来源：http://vro.316326.xyz

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://akz.yonumen.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://nes.yj20258.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nrd.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://blw.hammf.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gfr.0kj1m.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xuj.dianchejie.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dpu.dashuyun.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://csi.yangfankeji.com

[L04] 设置超时
来源：http://gow.jlsjyb.cn

Py:   requests.get(url, timeout=5)
来源：http://usx.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://djb.quarkkingdee.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yap.pycfn.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cms.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wsb.zhixingplan.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://stl.quarkkingdee.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pyo.pengpengdd.cyou

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ure.yongpay.top

[L05] 上传文件（multipart）
来源：http://wll.redwolf501.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ydl.yongpay.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://qyk.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lub.hesvh.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://vbz.chenzaomai.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dzq.nanxuanxn.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://joz.ywan-chungtsiang.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zpt.jiagoushi.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sgl.cqqwz.cn

[L06] 解析响应为 JSON
来源：http://jqt.fanxiaobao.xyz

Py:   resp.json()
来源：http://dyw.xuetiantiany.cn

PHP:  json_decode($body, true);
来源：http://cxl.jinyuanbaomall.cn

JS:   await resp.json()
来源：http://yob.hywenlv.cn

TS:   await resp.json()
来源：http://mfs.jqgfzy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://vlx.gogol.net.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://xkt.andypj.xyz

Ruby: JSON.parse(resp.body)
来源：http://now.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://whc.yueranfly.top

[L07] 处理 HTTP 状态码
来源：http://ece.shuidangran.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gva.redwolf501.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://dbq.zhongyouzk.top

JS:   resp.ok;  resp.status
来源：http://rul.dashuyun.cn

TS:   resp.ok;  resp.status
来源：http://nmu.zhoulong.xyz

Java: resp.statusCode()
来源：http://srh.shuidangran.top

Go:   resp.StatusCode
来源：http://gux.ydjk.org.cn

Ruby: resp.code.to_i
来源：http://tkd.redwolf501.top

C#:   (int)resp.StatusCode
来源：http://ixf.tarul.cn

[L08] 并发请求多个地址
来源：http://klj.shuidangran.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://chh.fanxiaobao.xyz

PHP:  curl_multi_init() 系列
来源：http://rfi.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vna.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://fdl.hfpthk.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vnq.yj20258.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://idq.xinyue.icu

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qkw.chenlongwang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://vjb.hnxiangtu.top

================================================================================
来源：http://anf.jqgufenzy.top

M. 命令行 / 进程 / 环境
来源：http://wyo.zhixingplan.top

================================================================================
来源：http://dye.shanyushiyangkeji.top

[M01] 读取命令行参数
来源：http://jgi.nanxuanxn.top

Py:   sys.argv[1:]
来源：http://rhg.jiagoushi.top

PHP:  $argv;  $argc;
来源：http://xup.shzxlz.cn

JS:   process.argv.slice(2)
来源：http://ypv.epnwcf.com

TS:   process.argv.slice(2)
来源：http://rbk.yvedp.cn

Java: args 数组（main 方法参数）
来源：http://wcf.guowangkeji.top

Go:   os.Args[1:]
来源：http://eji.yuxming.cn

Ruby: ARGV
来源：http://bwi.hywenlv.cn

C#:   args 数组（Main 方法参数）
来源：http://sdq.jinyuanbaomall.cn

[M02] 读取环境变量
来源：http://tde.hammf.cn

Py:   os.environ.get("HOME")
来源：http://jsf.ivvv.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bbt.jqgufenzy.top

JS:   process.env.HOME
来源：http://zif.hysaishi.cn

TS:   process.env.HOME
来源：http://hdu.dianchejie.cn

Java: System.getenv("HOME")
来源：http://mwn.nanxuanxn.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ujx.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://kup.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://scn.hcnkem.com

[M03] 执行外部命令
来源：http://gqu.haohaochexian.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://eih.yfazqb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://jpe.gzhubu.top

JS:   child_process.execSync("ls -l").toString()
来源：http://lws.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://aaf.iojbl.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nxj.yvedp.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xol.jlsjyb.cn

Ruby: system("ls -l");  `ls -l`
来源：http://dye.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://kid.jianghu66.top

[M04] 获取当前工作目录
来源：http://rrz.sjlbkw.cn

Py:   os.getcwd()
来源：http://sfa.hysaishi.cn

PHP:  getcwd();
来源：http://qsq.snrcjt.cn

JS:   process.cwd()
来源：http://zvr.jinqigfzy.top

TS:   process.cwd()
来源：http://enx.yueranfly.top

Java: Path.of("").toAbsolutePath()
来源：http://aoq.nanxinkj.top

Go:   os.Getwd()
来源：http://rba.xziqi.cn

Ruby: Dir.pwd
来源：http://lyp.yonumen.top

C#:   Directory.GetCurrentDirectory()
来源：http://xxk.vehdjk.com

[M05] 设置退出码
来源：http://gnk.hywenlv.cn

Py:   sys.exit(1)
来源：http://poz.zdbjq.cn

PHP:  exit(1);
来源：http://all.9152youxi.cn

JS:   process.exit(1)
来源：http://qst.nanxuanxn.top

TS:   process.exit(1)
来源：http://lja.nwbrower.top

Java: System.exit(1)
来源：http://qdu.jlsjyb.cn

Go:   os.Exit(1)
来源：http://owk.zhengqikj.top

Ruby: exit 1
来源：http://pos.sweek.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ron.yuanzhike.top

[M06] 向标准错误输出
来源：http://dqk.andypj.xyz

Py:   print("err", file=sys.stderr)
来源：http://nmf.cucudq.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://kal.316326.xyz

JS:   console.error("err")
来源：http://aem.zycfv.cn

TS:   console.error("err")
来源：http://ipp.wangdashe.top

Java: System.err.println("err")
来源：http://grr.zhengqikj.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://lpj.daxiang520.top

Ruby: warn "err"
来源：http://pua.zycfv.cn

C#:   Console.Error.WriteLine("err")
来源：http://dgd.ehwqpu.com

[M07] 判断是否为主入口
来源：http://rsx.gotoacloud.top

Py:   if __name__ == "__main__":
来源：http://you.vehdjk.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://kzz.pengpengdd.cyou

JS:   require.main === module
来源：http://kmr.haohaochexian.top

TS:   require.main === module
来源：http://yje.hesvh.cn

Java: public static void main(String[] args)
来源：http://wny.shzxlz.cn

Go:   func main()
来源：http://opy.yonumen.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://wvx.iojbl.cn

C#:   static void Main(string[] args)
来源：http://qaj.birdmap.top

[M08] 获取系统与运行时信息
来源：http://lll.yfazqb.com

Py:   platform.system();  platform.python_version()
来源：http://fax.wangdashe.top

PHP:  PHP_OS;  phpversion();
来源：http://ekq.fehbvm.com

JS:   process.platform;  process.version
来源：http://juo.sweek.top

TS:   process.platform;  process.version
来源：http://gzj.c1oappe.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wll.daxiang520.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://wqv.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://njx.shuidangran.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nfa.fanxiaobao.xyz

================================================================================
来源：http://jow.yongpay.top

N. 数据结构与算法
来源：http://ips.jinyuanbaomall.cn

================================================================================
来源：http://cjw.gaohongyu789.top

[N01] 二分查找（有序数组）
来源：http://sae.yuxming.cn

Py:   bisect.bisect_left(arr, x)
来源：http://amx.zhengqikj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wmx.sweek.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://oom.jiagoushi.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jvr.zhongyouzk.top

Java: Arrays.binarySearch(arr, x)
来源：http://wod.sjlbkw.cn

Go:   sort.SearchInts(arr, x)
来源：http://mpd.quarkkingdee.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hth.yj20258.top

C#:   Array.BinarySearch(arr, x)
来源：http://gfa.tianlin.xyz

[N02] 排序（工程实践用内置实现）
来源：http://rbz.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://cmi.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://uhu.smart0.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://tnd.kuanghao11.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dkg.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zoc.ppjwa.cn

Go:   slices.Sort(arr)
来源：http://pdf.yj20258.top

Ruby: arr.sort
来源：http://ogv.hongshengwenyu.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://qhn.fzhhl.top

[N03] 快速排序（分治示例）
来源：http://mea.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://jyq.yongpay.top

PHP:  // 递归实现，或用 usort
来源：http://hka.quarkkingdee.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://rpj.ppjwa.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qja.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://dzj.hysaishi.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://spj.tarul.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ffc.xuetiantiany.cn

C#:   // 手写递归，或 Array.Sort
来源：http://ryz.sufxvd.cn

[N04] 斐波那契数列
来源：http://vol.jinqigufen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rkr.redwolf501.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fbo.jlsjyb.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kdo.zdbjq.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://opb.cheryme.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://qjm.chenlongwang.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://odn.gzhubu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://vqm.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pmd.jqgufenzy.top

[N05] 最大公约数
来源：http://ion.gaohongyu789.top

Py:   math.gcd(a, b)
来源：http://pvr.bbcook.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://oia.bjfxy.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ect.jinqigfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ijn.jinyuanbaomall.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ydy.hesvh.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://glx.ctjpmb.com

Ruby: a.gcd(b)
来源：http://edy.sjlbkw.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://nzn.shanyushiyangkeji.top

[N06] 判断回文字符串
来源：http://vqw.xylfe.cn

Py:   s == s[::-1]
来源：http://lbj.daxiang520.top

PHP:  $s === strrev($s);
来源：http://kvh.fzhhl.top

JS:   s === [...s].reverse().join("")
来源：http://fqj.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://lzv.ctjpmb.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iee.9152youxi.cn

Go:   // 双指针从两端比较
来源：http://rgr.cqqwz.cn

Ruby: s == s.reverse
来源：http://sop.ivvv.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://fvo.chenjidiqi.icu

[N07] 两数之和（返回下标）
来源：http://alm.xuetiantiany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vtz.tianlin.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://bha.kuanghao11.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kkq.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://djx.chenjidiqi.icu

Java: // 手写 HashMap
来源：http://hwr.yvedp.cn


<!-- 参考信息 -->