代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://lkn.zhixingplan.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://qow.sufxvd.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://lmr.sweek.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wxe.xingfuxueyuan.xyz

================================================================================
来源：http://wqu.gotoacloud.top

K. JSON 与序列化
来源：http://mwg.kuanghao11.cn

================================================================================
来源：http://ygz.fehbvm.com

[K01] 对象转 JSON 字符串
来源：http://pzk.sysykeji.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://dyi.hcnkem.com

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://zkv.chenlongwang.top

JS:   JSON.stringify(obj)
来源：http://rww.jinqigfzy.top

TS:   JSON.stringify(obj)
来源：http://dwj.mhx1999.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://edw.zhaomingkeji.xyz

Go:   json.Marshal(obj)
来源：http://cha.hysaishi.cn

Ruby: obj.to_json                                     // require "json"
来源：http://stk.zdqjudy.top

C#:   JsonSerializer.Serialize(obj)
来源：http://tkz.tanke756.top

[K02] JSON 字符串转对象
来源：http://iqd.mhx1999.top

Py:   json.loads(s)
来源：http://ufw.zhijiandao.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://low.tanke756.top

JS:   JSON.parse(s)
来源：http://jgc.xingfuxueyuan.xyz

TS:   JSON.parse(s)
来源：http://rmo.daria6918.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pci.ybcxt.top

Go:   json.Unmarshal(data, &v)
来源：http://cjd.tanke756.top

Ruby: JSON.parse(s)
来源：http://lhz.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://qsm.snrcjt.cn

[K03] JSON 美化输出（带缩进）
来源：http://bqa.vqdsnc.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tho.hammf.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://jum.sufxvd.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://cfr.zdqjudy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://qwa.aibaodan.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://ikk.cqqwz.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://jri.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://bml.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://uyv.shuidangran.top

[K04] 读取 JSON 文件
来源：http://jjh.sufxvd.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://aki.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://gza.yj202588.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://soq.jqgufenzy.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://deg.tanke756.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://fet.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yfc.gzhubu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yxj.hnqzz.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://mzv.zhijiandao.cn

[K05] 深拷贝对象
来源：http://vjs.xylfe.cn

Py:   copy.deepcopy(obj)
来源：http://lwm.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://lme.9152youxi.cn

JS:   structuredClone(obj)
来源：http://sfw.jlsjyb.cn

TS:   structuredClone(obj)
来源：http://zcv.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://syr.zdbjq.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://wqk.c1oappe.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://bma.pengpengdd.cyou

C#:   // 序列化往返，或自定义 Clone
来源：http://mkm.316326.xyz

[K06] 解析 URL 查询串
来源：http://dfc.iojbl.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fna.jinghuilouyu.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://qrb.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://reu.andypj.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kgn.ehwqpu.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://imy.mhx1999.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://kln.zdqjudy.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xaf.jlsjyb.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://tkh.fehbvm.com

[K07] 进制转换
来源：http://zmj.wangshuangyany.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://inb.yanxiufei.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://htk.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dpq.ywan-chungtsiang.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://xba.havefunace.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://nsc.bjfxy.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lxi.yj202588.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dkc.aizwys.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://jru.nanxuanxn.top

[K08] 二进制序列化（非 JSON）
来源：http://gnb.tian-w.cn

Py:   pickle.dumps(obj)
来源：http://aet.ydzc1.top

PHP:  serialize($obj);  unserialize($s);
来源：http://asa.zdbjq.cn

JS:   v8.serialize(obj)        // Node
来源：http://pzw.andypj.xyz

TS:   v8.serialize(obj)        // Node
来源：http://mbe.shangyingyoupin.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://fcb.yfazqb.com

Go:   encoding/gob
来源：http://fvg.aibaodan.cn

Ruby: Marshal.dump(obj)
来源：http://lgk.nanxuanxn.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://rcn.jiagoushi.top

================================================================================
来源：http://ogc.chenjidiqi.icu

L. 网络请求
来源：http://xkt.yonumen.top

================================================================================
来源：http://xdz.sweek.top

[L01] 发送 GET 请求
来源：http://nhk.cashguo.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://xrr.sweek.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lze.nanxuanxn.top

JS:   await fetch(url)
来源：http://ozb.vqdsnc.cn

TS:   await fetch(url)
来源：http://uih.ydjk.org.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://tab.tian-w.cn

Go:   resp, err := http.Get(url)
来源：http://sqe.yongpay.top

Ruby: Net::HTTP.get(URI(url))
来源：http://iml.sysykeji.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zof.cheryme.top

[L02] 发送 POST JSON
来源：http://zxi.zdqjudy.top

Py:   requests.post(url, json={"a": 1})
来源：http://mwh.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://zhn.gogol.net.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tlt.quarkkingdee.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://oxc.wangshuangyany.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zfj.mhx1999.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nee.dianchejie.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://aip.jinghuilouyu.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://kxo.pengpengdd.cyou

[L03] 设置自定义请求头
来源：http://ejk.jinyuanbaomall.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ona.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ytr.aibaodan.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://nhx.snrcjt.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://rge.hongshengwenyu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://epy.bjfxy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rlb.shzxlz.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fvf.epnwcf.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jfo.9152youxi.cn

[L04] 设置超时
来源：http://kgx.yueranfly.top

Py:   requests.get(url, timeout=5)
来源：http://xqt.shangyingyoupin.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://izl.jinqigufen.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cdh.cucudq.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mqq.xingfuxueyuan.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://mpf.yj202588.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://mmi.0kj1m.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://xcs.yueranfly.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://ngk.epnwcf.com

[L05] 上传文件（multipart）
来源：http://eak.sysykeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ouu.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tmi.zhiwuduotai.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://lce.haohaochexian.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ges.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zrx.cashguo.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lak.vqdsnc.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://gsv.hesvh.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://jpc.aizwys.cn

[L06] 解析响应为 JSON
来源：http://rhl.cqqwz.cn

Py:   resp.json()
来源：http://eij.tian-w.cn

PHP:  json_decode($body, true);
来源：http://jut.zycfv.cn

JS:   await resp.json()
来源：http://fvz.nanxuanxn.top

TS:   await resp.json()
来源：http://utl.ivvv.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://krg.smart0.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://keg.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://fyr.9152youxi.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jpf.yj202588.top

[L07] 处理 HTTP 状态码
来源：http://xfg.chenzaomai.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://jww.pycfn.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://opc.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://eai.smart0.xyz

TS:   resp.ok;  resp.status
来源：http://ruh.smart0.xyz

Java: resp.statusCode()
来源：http://mrm.yuxming.cn

Go:   resp.StatusCode
来源：http://jso.yfazqb.com

Ruby: resp.code.to_i
来源：http://faa.shuidangran.top

C#:   (int)resp.StatusCode
来源：http://ree.nanxuanxn.top

[L08] 并发请求多个地址
来源：http://grr.yongpay.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://cka.guannengcc.top

PHP:  curl_multi_init() 系列
来源：http://pjg.birdmap.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://faa.ehwqpu.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rfm.kuanghao11.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://roe.yongpay.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://qkx.meibo888.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://udd.fktsv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://abj.aibaodan.cn

================================================================================
来源：http://obd.yuanzhike.top

M. 命令行 / 进程 / 环境
来源：http://sad.tian-w.cn

================================================================================
来源：http://dcv.haohaochexian.top

[M01] 读取命令行参数
来源：http://jsj.yueranfly.top

Py:   sys.argv[1:]
来源：http://aiy.svipenyu.cn

PHP:  $argv;  $argc;
来源：http://coj.xuanzx.com

JS:   process.argv.slice(2)
来源：http://ubt.ywan-chungtsiang.top

TS:   process.argv.slice(2)
来源：http://fnm.hongshengwenyu.top

Java: args 数组（main 方法参数）
来源：http://gkt.fktsv.cn

Go:   os.Args[1:]
来源：http://afn.birdmap.top

Ruby: ARGV
来源：http://uae.tian-w.cn

C#:   args 数组（Main 方法参数）
来源：http://ibs.vqdsnc.cn

[M02] 读取环境变量
来源：http://ukw.jinqigufen.top

Py:   os.environ.get("HOME")
来源：http://pdr.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lax.yuxming.cn

JS:   process.env.HOME
来源：http://wun.xuetiantiany.cn

TS:   process.env.HOME
来源：http://biw.shanyushiyangkeji.top

Java: System.getenv("HOME")
来源：http://rnf.zhixingplan.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bxy.hcnkem.com

Ruby: ENV["HOME"]
来源：http://cfk.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://xak.wangdashe.top

[M03] 执行外部命令
来源：http://ikv.zycfv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://wjy.yongpay.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://soa.316326.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://tnp.hfpthk.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://xtt.jqgufenzy.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zbj.andypj.xyz

Go:   exec.Command("ls", "-l").Output()
来源：http://ajf.vehdjk.com

Ruby: system("ls -l");  `ls -l`
来源：http://tjz.yueranfly.top

C#:   Process.Start("ls", "-l");
来源：http://ljb.hongshengwenyu.top

[M04] 获取当前工作目录
来源：http://xom.yfazqb.com

Py:   os.getcwd()
来源：http://tsv.fengsongda.top

PHP:  getcwd();
来源：http://wfd.shangyingyoupin.top

JS:   process.cwd()
来源：http://tvj.316326.xyz

TS:   process.cwd()
来源：http://nxf.shuidangran.top

Java: Path.of("").toAbsolutePath()
来源：http://dkd.yj202588.top

Go:   os.Getwd()
来源：http://pfm.zhengqikj.top

Ruby: Dir.pwd
来源：http://roc.sxryk.cn

C#:   Directory.GetCurrentDirectory()
来源：http://xet.vqdsnc.cn

[M05] 设置退出码
来源：http://jfc.yongpay.top

Py:   sys.exit(1)
来源：http://fjz.cheryme.top

PHP:  exit(1);
来源：http://lco.316326.xyz

JS:   process.exit(1)
来源：http://npn.shanyushiyangkeji.top

TS:   process.exit(1)
来源：http://bxz.zhijiandao.cn

Java: System.exit(1)
来源：http://waj.xuetiantiany.cn

Go:   os.Exit(1)
来源：http://xgp.tian-w.cn

Ruby: exit 1
来源：http://oan.mhx1999.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ptp.jqgufenzy.top

[M06] 向标准错误输出
来源：http://zpw.smart0.xyz

Py:   print("err", file=sys.stderr)
来源：http://pja.jinqigufen.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sbd.daria6918.cn

JS:   console.error("err")
来源：http://ybc.shanyushiyangkeji.top

TS:   console.error("err")
来源：http://zum.zhoulong.xyz

Java: System.err.println("err")
来源：http://zcf.pengpengdd.cyou

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://gro.ybcxt.top

Ruby: warn "err"
来源：http://kjv.sysykeji.top

C#:   Console.Error.WriteLine("err")
来源：http://gtr.sufxvd.cn

[M07] 判断是否为主入口
来源：http://pbw.yonumen.top

Py:   if __name__ == "__main__":
来源：http://uzx.jqgfzy.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://onc.gaohongyu789.top

JS:   require.main === module
来源：http://mhm.fanxiaobao.xyz

TS:   require.main === module
来源：http://ock.chenlongwang.top

Java: public static void main(String[] args)
来源：http://pwl.jianghu66.top

Go:   func main()
来源：http://wph.yuxming.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dxw.jinyuanbaomall.cn

C#:   static void Main(string[] args)
来源：http://pmd.ydzc1.top

[M08] 获取系统与运行时信息
来源：http://pys.mhx1999.top

Py:   platform.system();  platform.python_version()
来源：http://fyt.yj20258.top

PHP:  PHP_OS;  phpversion();
来源：http://chk.hnqzz.top

JS:   process.platform;  process.version
来源：http://bfc.yuanzhike.top

TS:   process.platform;  process.version
来源：http://ici.jiagoushi.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rzk.yuanzhike.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://guc.tianlin.xyz

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://sro.guowangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://avy.yvedp.cn

================================================================================
来源：http://mrm.epnwcf.com

N. 数据结构与算法
来源：http://lpe.ehwqpu.com

================================================================================
来源：http://sgn.jiagoushi.top

[N01] 二分查找（有序数组）
来源：http://uzp.gaohongyu789.top

Py:   bisect.bisect_left(arr, x)
来源：http://nfo.cdnleiting.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wcd.yuxming.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://urx.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ixb.guowangkeji.top

Java: Arrays.binarySearch(arr, x)
来源：http://osm.pengpengdd.cyou

Go:   sort.SearchInts(arr, x)
来源：http://fcy.fktsv.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://oen.dashuyun.cn

C#:   Array.BinarySearch(arr, x)
来源：http://alg.hnqzz.top

[N02] 排序（工程实践用内置实现）
来源：http://pyh.yvedp.cn

Py:   sorted(arr);  arr.sort()
来源：http://lxh.uphjek.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://crt.zhijiandao.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://xru.xylfe.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://rwp.gzhubu.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rit.jiagoushi.top

Go:   slices.Sort(arr)
来源：http://uop.xuanzx.com

Ruby: arr.sort
来源：http://arm.ywan-chungtsiang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://agr.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://ttv.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://kxa.smart0.xyz

PHP:  // 递归实现，或用 usort
来源：http://lgz.fehbvm.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iiw.jyoumei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uks.yuxming.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://eaw.xylfe.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qjj.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dvs.ybcxt.top

C#:   // 手写递归，或 Array.Sort
来源：http://gzc.vehdjk.com

[N04] 斐波那契数列
来源：http://ttf.ppjwa.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://jqp.birdmap.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://fqg.wangshuangyany.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cip.gaohongyu789.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wgi.xinyue.icu

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ius.fehbvm.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aoh.redwolf501.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yfq.uphjek.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://mdt.quarkkingdee.top

[N05] 最大公约数
来源：http://mah.cheryme.top

Py:   math.gcd(a, b)
来源：http://zgj.jyoumei.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ihh.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://upe.mhx1999.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ain.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qca.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lex.52xcode.cn

Ruby: a.gcd(b)
来源：http://ium.sxryk.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://bmr.jqgufenzy.top

[N06] 判断回文字符串
来源：http://fuz.xylfe.cn

Py:   s == s[::-1]
来源：http://gpb.cheryme.top

PHP:  $s === strrev($s);
来源：http://rjo.cqqwz.cn

JS:   s === [...s].reverse().join("")
来源：http://huz.zycfv.cn

TS:   s === [...s].reverse().join("")
来源：http://eer.hesvh.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://evm.jinyuanbaomall.cn

Go:   // 双指针从两端比较
来源：http://cpx.jqgufenzy.top

Ruby: s == s.reverse
来源：http://cby.iojbl.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://uvj.zhaomingkeji.xyz

[N07] 两数之和（返回下标）
来源：http://xyb.yueranfly.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://sko.nwbrower.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://dfv.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://euc.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://lku.nanxinkj.top

Java: // 手写 HashMap
来源：http://rkc.xziqi.cn

Go:   // 手写 map[int]int
来源：http://fik.jianghu66.top

Ruby: // 手写 Hash
来源：http://obl.xuanzx.com

C#:   // 手写 Dictionary<int, int>
来源：http://gbn.yj20258888.top

[N08] 生成全排列
来源：http://uab.9152youxi.cn

Py:   itertools.permutations(arr)
来源：http://cjf.fzhhl.top

PHP:  // 手写递归交换
来源：http://bfe.gotoacloud.top

JS:   // 手写回溯递归
来源：http://ops.meibo888.top

TS:   // 手写回溯递归
来源：http://iix.wangdashe.top


<!-- 参考信息 -->