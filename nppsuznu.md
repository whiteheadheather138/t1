代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://maq.dianchejie.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://upb.tian-w.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://vxj.aibaodan.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ogs.gogol.net.cn

================================================================================
来源：http://wex.zdqjudy.top

K. JSON 与序列化
来源：http://jmb.jinqigfzy.top

================================================================================
来源：http://dfw.nwbrower.top

[K01] 对象转 JSON 字符串
来源：http://lkc.chenlongwang.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://lxg.guannengcc.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://kbv.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://etc.c1oappe.top

TS:   JSON.stringify(obj)
来源：http://hey.cashguo.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xxc.nanxinkj.top

Go:   json.Marshal(obj)
来源：http://mvq.shanyushiyangkeji.top

Ruby: obj.to_json                                     // require "json"
来源：http://sqq.smart0.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://qyc.bjfxy.top

[K02] JSON 字符串转对象
来源：http://swi.chenzaomai.com

Py:   json.loads(s)
来源：http://xwo.meibo888.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://msy.daria6918.cn

JS:   JSON.parse(s)
来源：http://suc.xuetiantiany.cn

TS:   JSON.parse(s)
来源：http://lqw.andypj.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://mjq.316326.xyz

Go:   json.Unmarshal(data, &v)
来源：http://mgo.daxiang520.top

Ruby: JSON.parse(s)
来源：http://llw.yongpay.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cna.yueranfly.top

[K03] JSON 美化输出（带缩进）
来源：http://nrv.mhx1999.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cwd.zhengqikj.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://cmm.chenjidiqi.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://dtp.yj20258.top

TS:   JSON.stringify(obj, null, 2)
来源：http://lsc.yonumen.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rhw.aizwys.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://wdt.epnwcf.com

Ruby: JSON.pretty_generate(obj)
来源：http://est.zycfv.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kfg.ydjk.org.cn

[K04] 读取 JSON 文件
来源：http://mxe.aibaodan.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://rsd.hongshengwenyu.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xzk.ctjpmb.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ynd.fehbvm.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fjo.sysykeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://roh.dashuyun.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://lro.jqgufenzy.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://flb.ivvv.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tth.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://uik.sufxvd.cn

Py:   copy.deepcopy(obj)
来源：http://aet.quarkkingdee.top

PHP:  unserialize(serialize($obj));
来源：http://xni.sxryk.cn

JS:   structuredClone(obj)
来源：http://mgl.wangshuangyany.cn

TS:   structuredClone(obj)
来源：http://dal.xingfuxueyuan.xyz

Java: // 手写拷贝构造，或序列化往返
来源：http://mkm.svipenyu.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://zdi.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://aqo.kuanghao11.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ftn.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://ynq.shanyushiyangkeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://opp.wangshuangyany.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://eea.fktsv.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ztf.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kck.vehdjk.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://djb.chenzaomai.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://xql.ywan-chungtsiang.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://lsa.9152youxi.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://dnh.cdnleiting.top

[K07] 进制转换
来源：http://ruy.chenlongwang.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vmt.andypj.xyz

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://vgu.ydzc1.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://znd.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ryt.sweek.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://upv.ywan-chungtsiang.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://oyf.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://oio.jinqigufen.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ttq.chenzaomai.com

[K08] 二进制序列化（非 JSON）
来源：http://okw.shanyushiyangkeji.top

Py:   pickle.dumps(obj)
来源：http://nhp.svipenyu.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://qav.cheryme.top

JS:   v8.serialize(obj)        // Node
来源：http://piu.fengsongda.top

TS:   v8.serialize(obj)        // Node
来源：http://bas.guowangkeji.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fsi.chenjidiqi.icu

Go:   encoding/gob
来源：http://jrs.hnqzz.top

Ruby: Marshal.dump(obj)
来源：http://xdn.hammf.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://twc.jqgufenzy.top

================================================================================
来源：http://kot.zhixingplan.top

L. 网络请求
来源：http://eyf.hcnkem.com

================================================================================
来源：http://zbu.xylfe.cn

[L01] 发送 GET 请求
来源：http://yao.ydzc1.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://cmr.hnqzz.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://svs.svipenyu.cn

JS:   await fetch(url)
来源：http://nvz.0kj1m.cn

TS:   await fetch(url)
来源：http://qcj.shanyushiyangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hvk.shanyushiyangtech.top

Go:   resp, err := http.Get(url)
来源：http://mtx.zdbjq.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://hri.bbcook.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://kzw.ppjwa.cn

[L02] 发送 POST JSON
来源：http://pqm.fengsongda.top

Py:   requests.post(url, json={"a": 1})
来源：http://cwv.xuanzx.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://amy.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jcg.9152youxi.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rvm.zhiwuduotai.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ocx.sysykeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fnu.aibaodan.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://pfv.ctjpmb.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jhz.sufxvd.cn

[L03] 设置自定义请求头
来源：http://kpl.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ylu.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://lfy.snrcjt.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qgs.ctjpmb.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://txi.yanxiufei.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://yel.fengsongda.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rxn.yvedp.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tjp.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ouz.cdnleiting.top

[L04] 设置超时
来源：http://yrg.jinqigufen.top

Py:   requests.get(url, timeout=5)
来源：http://gyc.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ljm.tanke756.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://bli.ivvv.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ane.daria6918.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jbi.smart0.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zkd.hywenlv.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://gnk.snrcjt.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://skd.epnwcf.com

[L05] 上传文件（multipart）
来源：http://vai.hesvh.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yhp.fengsongda.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ztx.sufxvd.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kfk.jiagoushi.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://sgt.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fej.yonumen.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://fim.fktsv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://udf.hysaishi.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fvg.zycfv.cn

[L06] 解析响应为 JSON
来源：http://xja.zhixingplan.top

Py:   resp.json()
来源：http://zzx.nwbrower.top

PHP:  json_decode($body, true);
来源：http://cdy.jqgufenzy.top

JS:   await resp.json()
来源：http://gll.ydjk.org.cn

TS:   await resp.json()
来源：http://nxh.dashuyun.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ahs.fzhhl.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://fdt.shangyingyoupin.top

Ruby: JSON.parse(resp.body)
来源：http://qfo.sysykeji.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://dxw.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://ehp.9152youxi.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jzh.ywan-chungtsiang.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qqi.hongshengwenyu.top

JS:   resp.ok;  resp.status
来源：http://jzj.sysykeji.top

TS:   resp.ok;  resp.status
来源：http://fli.bjfxy.top

Java: resp.statusCode()
来源：http://nwc.ppjwa.cn

Go:   resp.StatusCode
来源：http://dfy.yonumen.top

Ruby: resp.code.to_i
来源：http://obh.zhengqikj.top

C#:   (int)resp.StatusCode
来源：http://xls.hfpthk.cn

[L08] 并发请求多个地址
来源：http://gct.xuetiantiany.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://lpb.ywan-chungtsiang.top

PHP:  curl_multi_init() 系列
来源：http://ouv.kuanghao11.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ilp.gogol.net.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://btx.52xcode.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qph.tarul.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://foz.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sxl.svipenyu.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ckr.vehdjk.com

================================================================================
来源：http://jji.nwbrower.top

M. 命令行 / 进程 / 环境
来源：http://brt.dashuyun.cn

================================================================================
来源：http://wvq.haohaochexian.top

[M01] 读取命令行参数
来源：http://qji.zhiwuduotai.top

Py:   sys.argv[1:]
来源：http://pwn.quarkkingdee.top

PHP:  $argv;  $argc;
来源：http://xha.yuxming.cn

JS:   process.argv.slice(2)
来源：http://ynl.zhoulong.xyz

TS:   process.argv.slice(2)
来源：http://tqv.shzxlz.cn

Java: args 数组（main 方法参数）
来源：http://loo.cqqwz.cn

Go:   os.Args[1:]
来源：http://tzk.yj202588.top

Ruby: ARGV
来源：http://rrk.meibo888.top

C#:   args 数组（Main 方法参数）
来源：http://akx.xinyue.icu

[M02] 读取环境变量
来源：http://tmq.0kj1m.cn

Py:   os.environ.get("HOME")
来源：http://shw.fehbvm.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://oyp.sjlbkw.cn

JS:   process.env.HOME
来源：http://ksi.havefunace.top

TS:   process.env.HOME
来源：http://mjc.yuxming.cn

Java: System.getenv("HOME")
来源：http://alj.sufxvd.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://jwt.tian-w.cn

Ruby: ENV["HOME"]
来源：http://tyz.tianlin.xyz

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fam.jiagoushi.top

[M03] 执行外部命令
来源：http://ytv.nwbrower.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fjb.jlsjyb.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ysu.zhiwuduotai.top

JS:   child_process.execSync("ls -l").toString()
来源：http://eze.epnwcf.com

TS:   child_process.execSync("ls -l").toString()
来源：http://esp.jlsjyb.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://owc.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://rgq.yfazqb.com

Ruby: system("ls -l");  `ls -l`
来源：http://tfu.jiagoushi.top

C#:   Process.Start("ls", "-l");
来源：http://dyd.snrcjt.cn

[M04] 获取当前工作目录
来源：http://rxx.zhijiandao.cn

Py:   os.getcwd()
来源：http://llt.ctjpmb.com

PHP:  getcwd();
来源：http://fca.sufxvd.cn

JS:   process.cwd()
来源：http://trp.tianlin.xyz

TS:   process.cwd()
来源：http://srk.guowangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://egy.quarkkingdee.top

Go:   os.Getwd()
来源：http://vqc.ivvv.top

Ruby: Dir.pwd
来源：http://ppq.yuanzhike.top

C#:   Directory.GetCurrentDirectory()
来源：http://tpi.yonumen.top

[M05] 设置退出码
来源：http://zhg.shzxlz.cn

Py:   sys.exit(1)
来源：http://rhu.cqqwz.cn

PHP:  exit(1);
来源：http://axt.xziqi.cn

JS:   process.exit(1)
来源：http://bgn.zhiwuduotai.top

TS:   process.exit(1)
来源：http://tju.redwolf501.top

Java: System.exit(1)
来源：http://lmi.tarul.cn

Go:   os.Exit(1)
来源：http://vxo.shangyingyoupin.top

Ruby: exit 1
来源：http://rur.shzxlz.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://gag.hywenlv.cn

[M06] 向标准错误输出
来源：http://szr.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://fux.zhaomingkeji.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://hns.yueranfly.top

JS:   console.error("err")
来源：http://noj.guowangkeji.top

TS:   console.error("err")
来源：http://lfr.yongpay.top

Java: System.err.println("err")
来源：http://tar.jlsjyb.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hcr.ywan-chungtsiang.top

Ruby: warn "err"
来源：http://zoh.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://syj.yj20258888.top

[M07] 判断是否为主入口
来源：http://hbz.hcnkem.com

Py:   if __name__ == "__main__":
来源：http://qen.yj20258888.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jzq.nanxuanxn.top

JS:   require.main === module
来源：http://iyr.smart0.xyz

TS:   require.main === module
来源：http://byp.yj202588.top

Java: public static void main(String[] args)
来源：http://bja.hnxiangtu.top

Go:   func main()
来源：http://ivi.zhaomingkeji.xyz

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://joz.ydzc1.top

C#:   static void Main(string[] args)
来源：http://bsq.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://pyk.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://izg.andypj.xyz

PHP:  PHP_OS;  phpversion();
来源：http://rqd.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://qan.xingfuxueyuan.xyz

TS:   process.platform;  process.version
来源：http://awf.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oqa.jqgufenzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lum.shanyushiyangtech.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ihw.316326.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://mff.ywan-chungtsiang.top

================================================================================
来源：http://ewq.guowangkeji.top

N. 数据结构与算法
来源：http://fnx.xingfuxueyuan.xyz

================================================================================
来源：http://fgu.uphjek.com

[N01] 二分查找（有序数组）
来源：http://kye.yj20258888.top

Py:   bisect.bisect_left(arr, x)
来源：http://ava.epnwcf.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zij.gaohongyu789.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ojo.ydjk.org.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ypi.gogol.net.cn

Java: Arrays.binarySearch(arr, x)
来源：http://kes.nwbrower.top

Go:   sort.SearchInts(arr, x)
来源：http://cgf.cheryme.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://spt.jyoumei.cn

C#:   Array.BinarySearch(arr, x)
来源：http://gog.hongshengwenyu.top

[N02] 排序（工程实践用内置实现）
来源：http://abi.birdmap.top

Py:   sorted(arr);  arr.sort()
来源：http://yfu.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://sbl.52xcode.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hre.sufxvd.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://fdp.zhongyouzk.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://euv.ywan-chungtsiang.top

Go:   slices.Sort(arr)
来源：http://gau.xziqi.cn

Ruby: arr.sort
来源：http://kfh.yongpay.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://fdr.cashguo.top

[N03] 快速排序（分治示例）
来源：http://mvs.9152youxi.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://rcy.yueranfly.top

PHP:  // 递归实现，或用 usort
来源：http://agu.ydjk.org.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://esh.cdnleiting.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hif.daxiang520.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://alv.wangdashe.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://tdq.gaohongyu789.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://slx.zhixingplan.top

C#:   // 手写递归，或 Array.Sort
来源：http://lqe.zhengqikj.top

[N04] 斐波那契数列
来源：http://myo.jqgfzy.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fbu.xingfuxueyuan.xyz

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://qbi.gotoacloud.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://kiv.zhaomingkeji.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ywi.cqqwz.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://apf.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://fob.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://geo.cdnleiting.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://xrj.guannengcc.top

[N05] 最大公约数
来源：http://yde.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://irf.yongpay.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://uum.shangyingyoupin.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://vix.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uen.sweek.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wog.hywenlv.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://dcq.ybcxt.top

Ruby: a.gcd(b)
来源：http://ndl.redwolf501.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://aqz.xylfe.cn

[N06] 判断回文字符串
来源：http://fvl.nanxinkj.top

Py:   s == s[::-1]
来源：http://kyt.gaohongyu789.top

PHP:  $s === strrev($s);
来源：http://kdi.zhaomingkeji.xyz

JS:   s === [...s].reverse().join("")
来源：http://hbf.yuanzhike.top

TS:   s === [...s].reverse().join("")
来源：http://znz.xuetiantiany.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://sde.iojbl.cn

Go:   // 双指针从两端比较
来源：http://koe.chenzaomai.com

Ruby: s == s.reverse
来源：http://esg.sjlbkw.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://oht.haohaochexian.top

[N07] 两数之和（返回下标）
来源：http://aja.yanxiufei.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://vlw.zhaomingkeji.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://fbu.shuidangran.top

JS:   // 手写 Map：map.set(v, i)
来源：http://tkg.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://ulr.zhijiandao.cn

Java: // 手写 HashMap
来源：http://jnf.ywan-chungtsiang.top

Go:   // 手写 map[int]int
来源：http://oup.zhijiandao.cn

Ruby: // 手写 Hash
来源：http://bbv.quarkkingdee.top

C#:   // 手写 Dictionary<int, int>
来源：http://ixm.c1oappe.top

[N08] 生成全排列
来源：http://lam.mhx1999.top

Py:   itertools.permutations(arr)
来源：http://yrj.vehdjk.com

PHP:  // 手写递归交换
来源：http://ywc.gogol.net.cn

JS:   // 手写回溯递归
来源：http://vnh.yuxming.cn

TS:   // 手写回溯递归
来源：http://koy.svipenyu.cn


<!-- 参考信息 -->