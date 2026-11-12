代发 wailian999

================================================================================
来源：http://kwr.jiagoushi.top

K. JSON 与序列化
来源：http://xbx.feifeiyinyue.top

================================================================================
来源：http://xuw.zhixingplan.top

[K01] 对象转 JSON 字符串
来源：http://msg.yongpay.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jsn.zhengqikj.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://jsk.jqgufenzy.top

JS:   JSON.stringify(obj)
来源：http://yzn.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://kto.yj20258.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bav.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://dlo.bbcook.cn

Ruby: obj.to_json                                     // require "json"
来源：http://cpa.hcnkem.com

C#:   JsonSerializer.Serialize(obj)
来源：http://lxb.sjlbkw.cn

[K02] JSON 字符串转对象
来源：http://wxy.jinqigufen.top

Py:   json.loads(s)
来源：http://goe.epnwcf.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ibu.svipenyu.cn

JS:   JSON.parse(s)
来源：http://qvj.shanyushiyangtech.top

TS:   JSON.parse(s)
来源：http://abj.hammf.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://ndy.jinqigfzy.top

Go:   json.Unmarshal(data, &v)
来源：http://etr.feifeiyinyue.top

Ruby: JSON.parse(s)
来源：http://bek.zhongyouzk.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ndn.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://ull.52xcode.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cdx.yj20258.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://emc.0kj1m.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://xlu.yueranfly.top

TS:   JSON.stringify(obj, null, 2)
来源：http://ebw.zycfv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://cgu.yj20258888.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://pit.haohaochexian.top

Ruby: JSON.pretty_generate(obj)
来源：http://cll.smart0.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://agy.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://eti.birdmap.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aau.smart0.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://hnd.xylfe.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ztf.chenjidiqi.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://has.chenzaomai.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://pyv.ydjk.org.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ocn.cashguo.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rqw.iojbl.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://yrg.dashuyun.cn

[K05] 深拷贝对象
来源：http://xol.52xcode.cn

Py:   copy.deepcopy(obj)
来源：http://ysz.ywan-chungtsiang.top

PHP:  unserialize(serialize($obj));
来源：http://hhs.ydjk.org.cn

JS:   structuredClone(obj)
来源：http://zle.zhixingplan.top

TS:   structuredClone(obj)
来源：http://ykd.wangdashe.top

Java: // 手写拷贝构造，或序列化往返
来源：http://auj.uphjek.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://gxc.sxryk.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uxg.sweek.top

C#:   // 序列化往返，或自定义 Clone
来源：http://kfr.zdbjq.cn

[K06] 解析 URL 查询串
来源：http://etv.aizwys.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://cjk.ydzc1.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hxr.sysykeji.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hyw.havefunace.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nin.haohaochexian.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://zvh.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://gnd.yj20258888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://tis.gogol.net.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wwc.zhiwuduotai.top

[K07] 进制转换
来源：http://dbo.daria6918.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qzv.dashuyun.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://xeu.yj20258.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://gzn.zhaomingkeji.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ofo.zhiwuduotai.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fdr.pengpengdd.cyou

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lqa.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://zpq.fzhhl.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ega.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://zvx.gogol.net.cn

Py:   pickle.dumps(obj)
来源：http://kmz.meibo888.top

PHP:  serialize($obj);  unserialize($s);
来源：http://hbl.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://mwu.tianlin.xyz

TS:   v8.serialize(obj)        // Node
来源：http://rfy.zdqjudy.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://mat.ivvv.top

Go:   encoding/gob
来源：http://fvn.nwbrower.top

Ruby: Marshal.dump(obj)
来源：http://bwm.zhongyouzk.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://deh.nwbrower.top

================================================================================
来源：http://nkb.yj202588.top

L. 网络请求
来源：http://dzy.yfazqb.com

================================================================================
来源：http://lfm.hongshengwenyu.top

[L01] 发送 GET 请求
来源：http://syt.ywan-chungtsiang.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rlv.yvedp.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://abu.yongpay.top

JS:   await fetch(url)
来源：http://lgl.xuetiantiany.cn

TS:   await fetch(url)
来源：http://nrj.yuxming.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://oxq.uphjek.com

Go:   resp, err := http.Get(url)
来源：http://lyd.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://kne.tianlin.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://aii.9152youxi.cn

[L02] 发送 POST JSON
来源：http://ewx.ywan-chungtsiang.top

Py:   requests.post(url, json={"a": 1})
来源：http://xko.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://kwp.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rjk.cheryme.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ecc.jqgfzy.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://dku.yfazqb.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://hft.ybcxt.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bnc.xinyue.icu

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://sqj.zhijiandao.cn

[L03] 设置自定义请求头
来源：http://zbs.zhiwuduotai.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://oda.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vsg.jinqigufen.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://haz.cashguo.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qew.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mer.wangshuangyany.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ska.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://zgw.shanyushiyangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hiz.9152youxi.cn

[L04] 设置超时
来源：http://uxp.yvedp.cn

Py:   requests.get(url, timeout=5)
来源：http://qzk.meibo888.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://opz.hywenlv.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ukv.52xcode.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zco.yongpay.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ysh.sysykeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://pvs.yj20258.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://epg.52xcode.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://vmq.jyoumei.cn

[L05] 上传文件（multipart）
来源：http://bpp.wangshuangyany.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://vwv.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://uqm.cashguo.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qia.hongshengwenyu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gfa.svipenyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://dmi.ywan-chungtsiang.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://cfw.ivvv.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://xgk.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jqp.nwbrower.top

[L06] 解析响应为 JSON
来源：http://vha.hnxiangtu.top

Py:   resp.json()
来源：http://rsw.svipenyu.cn

PHP:  json_decode($body, true);
来源：http://hkp.zhaomingkeji.xyz

JS:   await resp.json()
来源：http://cuz.smart0.xyz

TS:   await resp.json()
来源：http://gpq.jiagoushi.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zhb.shanyushiyangkeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://lul.jinyuanbaomall.cn

Ruby: JSON.parse(resp.body)
来源：http://ftb.gaohongyu789.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://rcb.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://ile.daria6918.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://dkg.bbcook.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vga.ppjwa.cn

JS:   resp.ok;  resp.status
来源：http://xsm.ehwqpu.com

TS:   resp.ok;  resp.status
来源：http://eld.yj20258888.top

Java: resp.statusCode()
来源：http://gnz.yuxming.cn

Go:   resp.StatusCode
来源：http://dix.sufxvd.cn

Ruby: resp.code.to_i
来源：http://nwc.guannengcc.top

C#:   (int)resp.StatusCode
来源：http://lsu.xylfe.cn

[L08] 并发请求多个地址
来源：http://tgu.ivvv.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dbf.shangyingyoupin.top

PHP:  curl_multi_init() 系列
来源：http://try.shanyushiyangkeji.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://mno.daxiang520.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ssb.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lgp.hesvh.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://iez.9152youxi.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vbx.ybcxt.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://gmk.zycfv.cn

================================================================================
来源：http://smz.hnxiangtu.top

M. 命令行 / 进程 / 环境
来源：http://yqs.ctjpmb.com

================================================================================
来源：http://fue.fengsongda.top

[M01] 读取命令行参数
来源：http://fyj.pengpengdd.cyou

Py:   sys.argv[1:]
来源：http://rhw.yonumen.top

PHP:  $argv;  $argc;
来源：http://yfz.ctjpmb.com

JS:   process.argv.slice(2)
来源：http://jru.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://qtb.daria6918.cn

Java: args 数组（main 方法参数）
来源：http://eek.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://hsq.cqqwz.cn

Ruby: ARGV
来源：http://jrm.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://vxb.xinyue.icu

[M02] 读取环境变量
来源：http://yer.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://poj.pycfn.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://ven.yuxming.cn

JS:   process.env.HOME
来源：http://azd.zdbjq.cn

TS:   process.env.HOME
来源：http://meo.zhaomingkeji.xyz

Java: System.getenv("HOME")
来源：http://fqk.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ptb.sufxvd.cn

Ruby: ENV["HOME"]
来源：http://rvk.wangshuangyany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yyw.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://hpn.cheryme.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://qpg.yfazqb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://gfy.hesvh.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://dsw.yongpay.top

TS:   child_process.execSync("ls -l").toString()
来源：http://woa.andypj.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://uxh.sxryk.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ujf.yanxiufei.cn

Ruby: system("ls -l");  `ls -l`
来源：http://pmk.fehbvm.com

C#:   Process.Start("ls", "-l");
来源：http://czs.jlsjyb.cn

[M04] 获取当前工作目录
来源：http://ioo.yanxiufei.cn

Py:   os.getcwd()
来源：http://qcl.316326.xyz

PHP:  getcwd();
来源：http://fkf.dashuyun.cn

JS:   process.cwd()
来源：http://whi.yongpay.top

TS:   process.cwd()
来源：http://xxa.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://jwz.quarkkingdee.top

Go:   os.Getwd()
来源：http://kyg.gzhubu.top

Ruby: Dir.pwd
来源：http://nhz.zhixingplan.top

C#:   Directory.GetCurrentDirectory()
来源：http://byj.vehdjk.com

[M05] 设置退出码
来源：http://ghm.cucudq.cn

Py:   sys.exit(1)
来源：http://ion.dianchejie.cn

PHP:  exit(1);
来源：http://zxt.yj202588.top

JS:   process.exit(1)
来源：http://rtr.bjfxy.top

TS:   process.exit(1)
来源：http://djv.meibo888.top

Java: System.exit(1)
来源：http://boy.yfazqb.com

Go:   os.Exit(1)
来源：http://xsu.fktsv.cn

Ruby: exit 1
来源：http://yso.yangfankeji.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://noy.zdbjq.cn

[M06] 向标准错误输出
来源：http://sfo.shangyingyoupin.top

Py:   print("err", file=sys.stderr)
来源：http://bga.jqgufenzy.top

PHP:  fwrite(STDERR, "err\n");
来源：http://vtq.gaohongyu789.top

JS:   console.error("err")
来源：http://kci.epnwcf.com

TS:   console.error("err")
来源：http://sii.mhx1999.top

Java: System.err.println("err")
来源：http://xoc.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://txw.snrcjt.cn

Ruby: warn "err"
来源：http://grf.xuetiantiany.cn

C#:   Console.Error.WriteLine("err")
来源：http://vxo.havefunace.top

[M07] 判断是否为主入口
来源：http://fzb.sxryk.cn

Py:   if __name__ == "__main__":
来源：http://qwf.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gme.zdbjq.cn

JS:   require.main === module
来源：http://fwx.cqqwz.cn

TS:   require.main === module
来源：http://ols.jyoumei.cn

Java: public static void main(String[] args)
来源：http://eko.havefunace.top

Go:   func main()
来源：http://yux.yfazqb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dbx.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://ond.jinqigfzy.top

[M08] 获取系统与运行时信息
来源：http://isn.yj202588.top

Py:   platform.system();  platform.python_version()
来源：http://fca.xylfe.cn

PHP:  PHP_OS;  phpversion();
来源：http://gzb.chenjidiqi.icu

JS:   process.platform;  process.version
来源：http://jtw.fanxiaobao.xyz

TS:   process.platform;  process.version
来源：http://nry.yonumen.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://blh.shzxlz.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://btg.yuanzhike.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://nuh.birdmap.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://vbs.yangfankeji.com

================================================================================
来源：http://wpt.ppjwa.cn

N. 数据结构与算法
来源：http://jxt.tian-w.cn

================================================================================
来源：http://jrs.zhaomingkeji.xyz

[N01] 二分查找（有序数组）
来源：http://yhk.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://rdt.shanyushiyangtech.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://org.kuanghao11.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ndw.wangshuangyany.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://umd.cheryme.top

Java: Arrays.binarySearch(arr, x)
来源：http://jkr.yj20258.top

Go:   sort.SearchInts(arr, x)
来源：http://kwo.xylfe.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://xkw.cheryme.top

C#:   Array.BinarySearch(arr, x)
来源：http://ise.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://gnc.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://wlj.hfpthk.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oap.fzhhl.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://wwy.ivvv.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://qwo.zhijiandao.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xpb.ybcxt.top

Go:   slices.Sort(arr)
来源：http://bie.jinqigufen.top

Ruby: arr.sort
来源：http://zkn.hesvh.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://exo.haohaochexian.top

[N03] 快速排序（分治示例）
来源：http://ffh.xingfuxueyuan.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nuz.cheryme.top

PHP:  // 递归实现，或用 usort
来源：http://ovb.shangyingyoupin.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ouw.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://asa.zdqjudy.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ysj.sxryk.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://txx.bbcook.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://vtd.yuxming.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jzo.havefunace.top

[N04] 斐波那契数列
来源：http://xfm.uphjek.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nwx.ydzc1.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://jow.jqgfzy.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fcf.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fsi.dashuyun.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://bke.havefunace.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dsu.havefunace.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ghp.sxryk.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://tfh.havefunace.top

[N05] 最大公约数
来源：http://hir.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://kfs.cheryme.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://srd.aibaodan.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://bbp.meibo888.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wsw.jqgfzy.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://gzk.yfazqb.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://zwn.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://vsn.tanke756.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qrd.havefunace.top

[N06] 判断回文字符串
来源：http://sob.hongshengwenyu.top

Py:   s == s[::-1]
来源：http://mmf.ybcxt.top

PHP:  $s === strrev($s);
来源：http://vuj.0kj1m.cn

JS:   s === [...s].reverse().join("")
来源：http://rrz.shanyushiyangtech.top

TS:   s === [...s].reverse().join("")
来源：http://tor.tianlin.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://rbp.daxiang520.top

Go:   // 双指针从两端比较
来源：http://vsq.ydzc1.top

Ruby: s == s.reverse
来源：http://tai.zhoulong.xyz

C#:   s == new string(s.Reverse().ToArray())
来源：http://bhj.daxiang520.top

[N07] 两数之和（返回下标）
来源：http://bec.cashguo.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wdy.xinyue.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://gyb.ppjwa.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://str.zhoulong.xyz

TS:   // 手写 Map<string, number>
来源：http://erp.sjlbkw.cn

Java: // 手写 HashMap
来源：http://kjf.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://jqa.nanxuanxn.top

Ruby: // 手写 Hash
来源：http://mpd.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://zmp.yueranfly.top

[N08] 生成全排列
来源：http://fkr.gaohongyu789.top

Py:   itertools.permutations(arr)
来源：http://ixs.wangshuangyany.cn

PHP:  // 手写递归交换
来源：http://xql.bbcook.cn

JS:   // 手写回溯递归
来源：http://yrd.epnwcf.com

TS:   // 手写回溯递归
来源：http://zgp.redwolf501.top

Java: // 手写回溯递归
来源：http://euq.hnqzz.top

Go:   // 手写回溯递归
来源：http://tmf.tian-w.cn

Ruby: arr.permutation.to_a
来源：http://ssv.andypj.xyz

C#:   // 手写回溯递归
来源：http://uqm.0kj1m.cn


<!-- 参考信息 -->