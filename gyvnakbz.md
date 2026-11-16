代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://top.cucudq.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://tzb.zhoulong.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://cfq.shanyushiyangkeji.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://efl.jiagoushi.top

================================================================================
来源：http://kgi.tian-w.cn

K. JSON 与序列化
来源：http://atj.meibo888.top

================================================================================
来源：http://www.daria6918.cn

[K01] 对象转 JSON 字符串
来源：http://zjn.hfpthk.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://ozr.gaohongyu789.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fuk.yongpay.top

JS:   JSON.stringify(obj)
来源：http://kpa.cqqwz.cn

TS:   JSON.stringify(obj)
来源：http://hos.birdmap.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://mdv.yuxming.cn

Go:   json.Marshal(obj)
来源：http://fxu.feifeiyinyue.top

Ruby: obj.to_json                                     // require "json"
来源：http://lco.jinghuilouyu.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ajp.fktsv.cn

[K02] JSON 字符串转对象
来源：http://iif.yongpay.top

Py:   json.loads(s)
来源：http://awp.yonumen.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://oiv.cheryme.top

JS:   JSON.parse(s)
来源：http://okg.zhongyouzk.top

TS:   JSON.parse(s)
来源：http://aap.jqgufenzy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vxx.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://sbf.ybcxt.top

Ruby: JSON.parse(s)
来源：http://btw.meibo888.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://oiy.chenlongwang.top

[K03] JSON 美化输出（带缩进）
来源：http://bbt.yanxiufei.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rxj.gogol.net.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://vis.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://rzq.gzhubu.top

TS:   JSON.stringify(obj, null, 2)
来源：http://igk.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://glc.tianlin.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://fgq.xuanzx.com

Ruby: JSON.pretty_generate(obj)
来源：http://bsj.sufxvd.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ska.fktsv.cn

[K04] 读取 JSON 文件
来源：http://bbo.hcnkem.com

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jkc.zhiwuduotai.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ivi.gzhubu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://uep.shuidangran.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nmf.gogol.net.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yuc.yvedp.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mwn.hammf.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://hcz.fktsv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://dok.zhengqikj.top

[K05] 深拷贝对象
来源：http://rdq.yuanzhike.top

Py:   copy.deepcopy(obj)
来源：http://wik.mhx1999.top

PHP:  unserialize(serialize($obj));
来源：http://tic.zdbjq.cn

JS:   structuredClone(obj)
来源：http://nnd.smart0.xyz

TS:   structuredClone(obj)
来源：http://ddy.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ogz.cqqwz.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://asd.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://mhq.zhixingplan.top

C#:   // 序列化往返，或自定义 Clone
来源：http://smp.jiagoushi.top

[K06] 解析 URL 查询串
来源：http://llu.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://oew.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nvs.ppjwa.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gwt.hongshengwenyu.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xfu.hammf.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://neq.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://dxd.svipenyu.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hng.zhijiandao.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tcs.yangfankeji.com

[K07] 进制转换
来源：http://jjy.fengsongda.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ywm.jinghuilouyu.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hkq.bjfxy.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://jsa.ydjk.org.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://fvd.shzxlz.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fji.hesvh.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wgj.meibo888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://brf.ybcxt.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tgs.ehwqpu.com

[K08] 二进制序列化（非 JSON）
来源：http://klu.snrcjt.cn

Py:   pickle.dumps(obj)
来源：http://arj.pycfn.com

PHP:  serialize($obj);  unserialize($s);
来源：http://fgq.ppjwa.cn

JS:   v8.serialize(obj)        // Node
来源：http://jwz.xziqi.cn

TS:   v8.serialize(obj)        // Node
来源：http://npj.pengpengdd.cyou

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jjv.xuanzx.com

Go:   encoding/gob
来源：http://ayj.jqgfzy.top

Ruby: Marshal.dump(obj)
来源：http://qfb.chenlongwang.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://xgf.pengpengdd.cyou

================================================================================
来源：http://lkp.iojbl.cn

L. 网络请求
来源：http://xni.mhx1999.top

================================================================================
来源：http://zsp.316326.xyz

[L01] 发送 GET 请求
来源：http://lge.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tds.fengsongda.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://bzr.hammf.cn

JS:   await fetch(url)
来源：http://ear.ywan-chungtsiang.top

TS:   await fetch(url)
来源：http://epz.birdmap.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wkm.sxryk.cn

Go:   resp, err := http.Get(url)
来源：http://hst.fzhhl.top

Ruby: Net::HTTP.get(URI(url))
来源：http://mfx.dianchejie.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://oxd.yuanzhike.top

[L02] 发送 POST JSON
来源：http://gyv.tianlin.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://qiv.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://hul.jinyuanbaomall.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lvq.feifeiyinyue.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uvd.sysykeji.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://mxd.svipenyu.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wqq.yvedp.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xde.vqdsnc.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://wjc.xinyue.icu

[L03] 设置自定义请求头
来源：http://rfn.yueranfly.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tpr.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://avt.zhijiandao.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://acz.fanxiaobao.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wdo.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://red.316326.xyz

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://nyz.feifeiyinyue.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://smi.yuxming.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fda.bjfxy.top

[L04] 设置超时
来源：http://vum.wangshuangyany.cn

Py:   requests.get(url, timeout=5)
来源：http://mtg.9152youxi.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ppn.cashguo.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mdr.shanyushiyangkeji.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://eyt.hongshengwenyu.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://owv.fanxiaobao.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://arw.tianlin.xyz

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kwc.hfpthk.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bzr.guannengcc.top

[L05] 上传文件（multipart）
来源：http://zib.chenzaomai.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://kwq.hysaishi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cpn.iojbl.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wpb.cashguo.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://kcz.316326.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://uug.fktsv.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lgv.snrcjt.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://slx.jqgfzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://pvf.9152youxi.cn

[L06] 解析响应为 JSON
来源：http://fpu.feifeiyinyue.top

Py:   resp.json()
来源：http://yqg.sjlbkw.cn

PHP:  json_decode($body, true);
来源：http://gck.hfpthk.cn

JS:   await resp.json()
来源：http://vio.hcnkem.com

TS:   await resp.json()
来源：http://gee.hysaishi.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mex.haohaochexian.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kip.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://ele.zhijiandao.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sir.ydzc1.top

[L07] 处理 HTTP 状态码
来源：http://nak.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://xas.zycfv.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nbt.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://nzx.chenzaomai.com

TS:   resp.ok;  resp.status
来源：http://mhz.hnxiangtu.top

Java: resp.statusCode()
来源：http://ofk.jiagoushi.top

Go:   resp.StatusCode
来源：http://rfb.zhengqikj.top

Ruby: resp.code.to_i
来源：http://fxc.epnwcf.com

C#:   (int)resp.StatusCode
来源：http://qcv.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://zjk.meibo888.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://jlv.fengsongda.top

PHP:  curl_multi_init() 系列
来源：http://jxz.yueranfly.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dkv.fehbvm.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zmz.sjlbkw.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://knc.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xgf.shuidangran.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dto.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://uzy.cucudq.cn

================================================================================
来源：http://fwz.ctjpmb.com

M. 命令行 / 进程 / 环境
来源：http://lum.uphjek.com

================================================================================
来源：http://ibr.nanxinkj.top

[M01] 读取命令行参数
来源：http://orl.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://rrp.yj202588.top

PHP:  $argv;  $argc;
来源：http://yla.hnxiangtu.top

JS:   process.argv.slice(2)
来源：http://qgg.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://zrv.zdbjq.cn

Java: args 数组（main 方法参数）
来源：http://unf.zhixingplan.top

Go:   os.Args[1:]
来源：http://mhu.daxiang520.top

Ruby: ARGV
来源：http://idd.xylfe.cn

C#:   args 数组（Main 方法参数）
来源：http://nlk.redwolf501.top

[M02] 读取环境变量
来源：http://fvy.vehdjk.com

Py:   os.environ.get("HOME")
来源：http://agh.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://klz.shanyushiyangkeji.top

JS:   process.env.HOME
来源：http://yss.cqqwz.cn

TS:   process.env.HOME
来源：http://scc.ywan-chungtsiang.top

Java: System.getenv("HOME")
来源：http://kmi.zycfv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://lap.fzhhl.top

Ruby: ENV["HOME"]
来源：http://tes.jinyuanbaomall.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lhx.xuanzx.com

[M03] 执行外部命令
来源：http://efy.nanxuanxn.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mep.c1oappe.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://sav.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://hau.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://okt.yj20258.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://fpc.hnqzz.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mqh.jinqigfzy.top

Ruby: system("ls -l");  `ls -l`
来源：http://jso.nanxinkj.top

C#:   Process.Start("ls", "-l");
来源：http://znf.gogol.net.cn

[M04] 获取当前工作目录
来源：http://obb.sysykeji.top

Py:   os.getcwd()
来源：http://llq.shanyushiyangkeji.top

PHP:  getcwd();
来源：http://xlu.zhiwuduotai.top

JS:   process.cwd()
来源：http://jer.bbcook.cn

TS:   process.cwd()
来源：http://vks.cqqwz.cn

Java: Path.of("").toAbsolutePath()
来源：http://mks.chenzaomai.com

Go:   os.Getwd()
来源：http://jtt.zhoulong.xyz

Ruby: Dir.pwd
来源：http://gfx.zdqjudy.top

C#:   Directory.GetCurrentDirectory()
来源：http://drj.redwolf501.top

[M05] 设置退出码
来源：http://blr.ybcxt.top

Py:   sys.exit(1)
来源：http://phr.jinyuanbaomall.cn

PHP:  exit(1);
来源：http://ayc.ydjk.org.cn

JS:   process.exit(1)
来源：http://wbb.iojbl.cn

TS:   process.exit(1)
来源：http://mah.fanxiaobao.xyz

Java: System.exit(1)
来源：http://qxl.dashuyun.cn

Go:   os.Exit(1)
来源：http://ofk.sjlbkw.cn

Ruby: exit 1
来源：http://ebg.9152youxi.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://jko.shuidangran.top

[M06] 向标准错误输出
来源：http://ork.jianghu66.top

Py:   print("err", file=sys.stderr)
来源：http://crl.snrcjt.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://nwh.birdmap.top

JS:   console.error("err")
来源：http://kkq.yj202588.top

TS:   console.error("err")
来源：http://bct.hfpthk.cn

Java: System.err.println("err")
来源：http://miv.xuanzx.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bkf.shangyingyoupin.top

Ruby: warn "err"
来源：http://dze.iojbl.cn

C#:   Console.Error.WriteLine("err")
来源：http://ops.fanxiaobao.xyz

[M07] 判断是否为主入口
来源：http://xlr.iojbl.cn

Py:   if __name__ == "__main__":
来源：http://twx.shanyushiyangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ooy.jinyuanbaomall.cn

JS:   require.main === module
来源：http://adx.chenjidiqi.icu

TS:   require.main === module
来源：http://tsh.bjfxy.top

Java: public static void main(String[] args)
来源：http://lsd.guowangkeji.top

Go:   func main()
来源：http://kvn.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://jpm.sxryk.cn

C#:   static void Main(string[] args)
来源：http://lqz.9152youxi.cn

[M08] 获取系统与运行时信息
来源：http://fyp.xuetiantiany.cn

Py:   platform.system();  platform.python_version()
来源：http://ptu.yvedp.cn

PHP:  PHP_OS;  phpversion();
来源：http://rly.nwbrower.top

JS:   process.platform;  process.version
来源：http://efn.xylfe.cn

TS:   process.platform;  process.version
来源：http://pvz.hfpthk.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nhr.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dtg.hnqzz.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gxy.feifeiyinyue.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://igw.dianchejie.cn

================================================================================
来源：http://yut.cucudq.cn

N. 数据结构与算法
来源：http://inz.hnqzz.top

================================================================================
来源：http://oqk.aibaodan.cn

[N01] 二分查找（有序数组）
来源：http://siy.epnwcf.com

Py:   bisect.bisect_left(arr, x)
来源：http://fdh.mhx1999.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://win.sysykeji.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://siy.yanxiufei.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xvh.hysaishi.cn

Java: Arrays.binarySearch(arr, x)
来源：http://uhb.shzxlz.cn

Go:   sort.SearchInts(arr, x)
来源：http://bou.tian-w.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://whj.zhiwuduotai.top

C#:   Array.BinarySearch(arr, x)
来源：http://ony.mhx1999.top

[N02] 排序（工程实践用内置实现）
来源：http://alt.ybcxt.top

Py:   sorted(arr);  arr.sort()
来源：http://wja.shanyushiyangtech.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://lud.hammf.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://pol.hnqzz.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qlx.chenjidiqi.icu

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://jzg.yangfankeji.com

Go:   slices.Sort(arr)
来源：http://psb.nanxinkj.top

Ruby: arr.sort
来源：http://obr.jinqigfzy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://uen.52xcode.cn

[N03] 快速排序（分治示例）
来源：http://wjn.ctjpmb.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://muh.epnwcf.com

PHP:  // 递归实现，或用 usort
来源：http://soj.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ckq.jqgufenzy.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://viv.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xlz.cashguo.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://oqc.bjfxy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://clz.cheryme.top

C#:   // 手写递归，或 Array.Sort
来源：http://mpl.jinqigfzy.top

[N04] 斐波那契数列
来源：http://qzz.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://iiz.daria6918.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://lxx.yj20258888.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cvk.hesvh.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mvi.wangdashe.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://zei.bbcook.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://iot.jinqigufen.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ane.yuanzhike.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://gzs.chenzaomai.com

[N05] 最大公约数
来源：http://erv.smart0.xyz

Py:   math.gcd(a, b)
来源：http://eaz.yangfankeji.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://guw.hammf.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ylv.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nux.xinyue.icu

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://sjs.yanxiufei.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://cpd.andypj.xyz

Ruby: a.gcd(b)
来源：http://eau.nanxinkj.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mjb.zhaomingkeji.xyz

[N06] 判断回文字符串
来源：http://ghk.zhoulong.xyz

Py:   s == s[::-1]
来源：http://ctn.hnxiangtu.top

PHP:  $s === strrev($s);
来源：http://ykb.chenjidiqi.icu

JS:   s === [...s].reverse().join("")
来源：http://chd.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://afl.haohaochexian.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qla.xinyue.icu

Go:   // 双指针从两端比较
来源：http://nfz.xziqi.cn

Ruby: s == s.reverse
来源：http://lci.hywenlv.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://mvb.shuidangran.top

[N07] 两数之和（返回下标）
来源：http://mvg.xziqi.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xtk.ydzc1.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rxs.aibaodan.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://lgp.jianghu66.top

TS:   // 手写 Map<string, number>
来源：http://hlj.xziqi.cn

Java: // 手写 HashMap
来源：http://die.gzhubu.top

Go:   // 手写 map[int]int
来源：http://tvp.tian-w.cn

Ruby: // 手写 Hash
来源：http://cfb.shanyushiyangkeji.top

C#:   // 手写 Dictionary<int, int>
来源：http://xys.jlsjyb.cn

[N08] 生成全排列
来源：http://gbg.jinghuilouyu.cn

Py:   itertools.permutations(arr)
来源：http://cdp.jqgufenzy.top

PHP:  // 手写递归交换
来源：http://jpv.9152youxi.cn

JS:   // 手写回溯递归
来源：http://ikn.c1oappe.top

TS:   // 手写回溯递归
来源：http://hxg.gogol.net.cn


<!-- 参考信息 -->