代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dsc.svipenyu.cn

Go:   json.Marshal(obj)
来源：http://kfq.c1oappe.top

Ruby: obj.to_json                                     // require "json"
来源：http://cxw.hywenlv.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fcs.cashguo.top

[K02] JSON 字符串转对象
来源：http://sia.jyoumei.cn

Py:   json.loads(s)
来源：http://hzd.nanxuanxn.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://txv.svipenyu.cn

JS:   JSON.parse(s)
来源：http://zwx.zdqjudy.top

TS:   JSON.parse(s)
来源：http://prc.havefunace.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bmh.c1oappe.top

Go:   json.Unmarshal(data, &v)
来源：http://thd.kuanghao11.cn

Ruby: JSON.parse(s)
来源：http://nli.jinqigfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ezy.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://xqw.quarkkingdee.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cuu.jlsjyb.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://nrt.hywenlv.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rji.wangdashe.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tij.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://dfq.jinqigufen.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://soa.fehbvm.com

Ruby: JSON.pretty_generate(obj)
来源：http://nal.chenlongwang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://gnu.chenjidiqi.icu

[K04] 读取 JSON 文件
来源：http://wac.yvedp.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://npb.fengsongda.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://kac.hammf.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ezb.aizwys.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://opb.yangfankeji.com

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://xgx.jlsjyb.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://wds.hfpthk.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://ujl.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rqc.meibo888.top

[K05] 深拷贝对象
来源：http://pjl.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://ghd.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://trq.vehdjk.com

JS:   structuredClone(obj)
来源：http://rwp.xylfe.cn

TS:   structuredClone(obj)
来源：http://cvb.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://btv.ppjwa.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ddk.hammf.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wmy.yonumen.top

C#:   // 序列化往返，或自定义 Clone
来源：http://fsc.yuanzhike.top

[K06] 解析 URL 查询串
来源：http://kro.yj20258.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://huc.sxryk.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://oyv.iojbl.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jpk.nanxinkj.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://had.shanyushiyangtech.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://fpq.cdnleiting.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://lio.fengsongda.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://oij.nanxuanxn.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://mmq.yanxiufei.cn

[K07] 进制转换
来源：http://fuo.316326.xyz

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://zha.hesvh.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://jnr.hongshengwenyu.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://hvd.sufxvd.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://seh.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lem.xinyue.icu

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://zuy.shzxlz.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://orx.yj20258888.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://aso.gzhubu.top

[K08] 二进制序列化（非 JSON）
来源：http://vxr.fktsv.cn

Py:   pickle.dumps(obj)
来源：http://skm.yonumen.top

PHP:  serialize($obj);  unserialize($s);
来源：http://idu.epnwcf.com

JS:   v8.serialize(obj)        // Node
来源：http://oyo.jlsjyb.cn

TS:   v8.serialize(obj)        // Node
来源：http://lrf.havefunace.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://smh.nwbrower.top

Go:   encoding/gob
来源：http://ron.gaohongyu789.top

Ruby: Marshal.dump(obj)
来源：http://tli.pengpengdd.cyou

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://gcb.shuidangran.top

================================================================================
来源：http://yvn.chenjidiqi.icu

L. 网络请求
来源：http://tcp.jianghu66.top

================================================================================
来源：http://dua.dianchejie.cn

[L01] 发送 GET 请求
来源：http://kon.jqgfzy.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sfr.hesvh.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sdh.wangdashe.top

JS:   await fetch(url)
来源：http://mgz.guowangkeji.top

TS:   await fetch(url)
来源：http://tsg.0kj1m.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bzo.wangshuangyany.cn

Go:   resp, err := http.Get(url)
来源：http://dxu.zhengqikj.top

Ruby: Net::HTTP.get(URI(url))
来源：http://scz.yonumen.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://abg.ydjk.org.cn

[L02] 发送 POST JSON
来源：http://spr.havefunace.top

Py:   requests.post(url, json={"a": 1})
来源：http://nvj.pengpengdd.cyou

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lla.chenlongwang.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tfs.chenzaomai.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://imp.pengpengdd.cyou

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://clc.cucudq.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ydr.zhixingplan.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ofg.chenlongwang.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bum.yanxiufei.cn

[L03] 设置自定义请求头
来源：http://kiw.tarul.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://xxx.jqgufenzy.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yhq.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fug.dashuyun.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cms.ywan-chungtsiang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dyc.zdqjudy.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://yhh.nwbrower.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://trg.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://lqi.shangyingyoupin.top

[L04] 设置超时
来源：http://ujf.svipenyu.cn

Py:   requests.get(url, timeout=5)
来源：http://zpg.fehbvm.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ifs.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fdi.gogol.net.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vhb.wangdashe.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://sug.0kj1m.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zhw.xuetiantiany.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://aqb.fengsongda.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qcs.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://wca.hongshengwenyu.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wns.jqgfzy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://jmy.meibo888.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://ded.gaohongyu789.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ypd.zhongyouzk.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yie.havefunace.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://oxg.nwbrower.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fao.hcnkem.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://asz.epnwcf.com

[L06] 解析响应为 JSON
来源：http://spm.tian-w.cn

Py:   resp.json()
来源：http://jhb.snrcjt.cn

PHP:  json_decode($body, true);
来源：http://vyo.nanxinkj.top

JS:   await resp.json()
来源：http://ndc.shanyushiyangtech.top

TS:   await resp.json()
来源：http://goj.yj20258888.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mtu.yj202588.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://foj.dianchejie.cn

Ruby: JSON.parse(resp.body)
来源：http://lcv.vehdjk.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://uti.dianchejie.cn

[L07] 处理 HTTP 状态码
来源：http://pqj.xylfe.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://mts.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://qka.snrcjt.cn

JS:   resp.ok;  resp.status
来源：http://mql.yongpay.top

TS:   resp.ok;  resp.status
来源：http://odz.jlsjyb.cn

Java: resp.statusCode()
来源：http://xxt.gaohongyu789.top

Go:   resp.StatusCode
来源：http://suc.fzhhl.top

Ruby: resp.code.to_i
来源：http://rin.52xcode.cn

C#:   (int)resp.StatusCode
来源：http://ywy.jianghu66.top

[L08] 并发请求多个地址
来源：http://osi.ivvv.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://zpc.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://ivp.havefunace.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://udy.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lgd.zhixingplan.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://vuc.hywenlv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://pej.hnxiangtu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://jls.vqdsnc.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://xbc.gotoacloud.top

================================================================================
来源：http://toe.sweek.top

M. 命令行 / 进程 / 环境
来源：http://hae.andypj.xyz

================================================================================
来源：http://ner.yueranfly.top

[M01] 读取命令行参数
来源：http://chg.shuidangran.top

Py:   sys.argv[1:]
来源：http://sla.52xcode.cn

PHP:  $argv;  $argc;
来源：http://mbk.hfpthk.cn

JS:   process.argv.slice(2)
来源：http://grn.yangfankeji.com

TS:   process.argv.slice(2)
来源：http://uhm.sjlbkw.cn

Java: args 数组（main 方法参数）
来源：http://lfq.daxiang520.top

Go:   os.Args[1:]
来源：http://utg.nwbrower.top

Ruby: ARGV
来源：http://foz.gzhubu.top

C#:   args 数组（Main 方法参数）
来源：http://bzc.jyoumei.cn

[M02] 读取环境变量
来源：http://qny.sysykeji.top

Py:   os.environ.get("HOME")
来源：http://ezl.yuanzhike.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bev.shzxlz.cn

JS:   process.env.HOME
来源：http://rnq.jianghu66.top

TS:   process.env.HOME
来源：http://did.daxiang520.top

Java: System.getenv("HOME")
来源：http://het.chenzaomai.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://djh.zycfv.cn

Ruby: ENV["HOME"]
来源：http://fwn.tian-w.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://drr.9152youxi.cn

[M03] 执行外部命令
来源：http://fvu.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dbr.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ayr.yanxiufei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://isw.gotoacloud.top

TS:   child_process.execSync("ls -l").toString()
来源：http://not.feifeiyinyue.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://olo.hesvh.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://mzm.ydzc1.top

Ruby: system("ls -l");  `ls -l`
来源：http://rpj.yvedp.cn

C#:   Process.Start("ls", "-l");
来源：http://nla.fktsv.cn

[M04] 获取当前工作目录
来源：http://khz.316326.xyz

Py:   os.getcwd()
来源：http://vni.hongshengwenyu.top

PHP:  getcwd();
来源：http://gae.dianchejie.cn

JS:   process.cwd()
来源：http://osx.ydjk.org.cn

TS:   process.cwd()
来源：http://yir.jinqigufen.top

Java: Path.of("").toAbsolutePath()
来源：http://qmz.aibaodan.cn

Go:   os.Getwd()
来源：http://dmi.dianchejie.cn

Ruby: Dir.pwd
来源：http://svr.haohaochexian.top

C#:   Directory.GetCurrentDirectory()
来源：http://any.guowangkeji.top

[M05] 设置退出码
来源：http://rxf.gogol.net.cn

Py:   sys.exit(1)
来源：http://uwf.sweek.top

PHP:  exit(1);
来源：http://qon.jianghu66.top

JS:   process.exit(1)
来源：http://ocs.jianghu66.top

TS:   process.exit(1)
来源：http://wpo.mhx1999.top

Java: System.exit(1)
来源：http://hfk.jlsjyb.cn

Go:   os.Exit(1)
来源：http://rqm.epnwcf.com

Ruby: exit 1
来源：http://gmi.jqgfzy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mgd.pycfn.com

[M06] 向标准错误输出
来源：http://asy.ppjwa.cn

Py:   print("err", file=sys.stderr)
来源：http://sql.quarkkingdee.top

PHP:  fwrite(STDERR, "err\n");
来源：http://xqs.cashguo.top

JS:   console.error("err")
来源：http://gel.birdmap.top

TS:   console.error("err")
来源：http://hnp.wangshuangyany.cn

Java: System.err.println("err")
来源：http://ive.ydzc1.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ebi.shanyushiyangtech.top

Ruby: warn "err"
来源：http://mqr.uphjek.com

C#:   Console.Error.WriteLine("err")
来源：http://ujc.epnwcf.com

[M07] 判断是否为主入口
来源：http://gpl.bjfxy.top

Py:   if __name__ == "__main__":
来源：http://dsv.dianchejie.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://bko.cucudq.cn

JS:   require.main === module
来源：http://luy.quarkkingdee.top

TS:   require.main === module
来源：http://bcm.ydjk.org.cn

Java: public static void main(String[] args)
来源：http://qyb.andypj.xyz

Go:   func main()
来源：http://okv.tarul.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://irx.tian-w.cn

C#:   static void Main(string[] args)
来源：http://wox.gogol.net.cn

[M08] 获取系统与运行时信息
来源：http://mkq.jianghu66.top

Py:   platform.system();  platform.python_version()
来源：http://rmt.daria6918.cn

PHP:  PHP_OS;  phpversion();
来源：http://ori.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://daf.fktsv.cn

TS:   process.platform;  process.version
来源：http://rzd.zycfv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://oox.birdmap.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://uyq.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://gnr.sysykeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lyd.gzhubu.top

================================================================================
来源：http://luk.fzhhl.top

N. 数据结构与算法
来源：http://wdm.shangyingyoupin.top

================================================================================
来源：http://utv.zhijiandao.cn

[N01] 二分查找（有序数组）
来源：http://max.yonumen.top

Py:   bisect.bisect_left(arr, x)
来源：http://sdx.52xcode.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://npb.ehwqpu.com

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tet.daria6918.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://dty.redwolf501.top

Java: Arrays.binarySearch(arr, x)
来源：http://ivl.jinghuilouyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://rpv.gogol.net.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iie.xinyue.icu

C#:   Array.BinarySearch(arr, x)
来源：http://uth.cdnleiting.top

[N02] 排序（工程实践用内置实现）
来源：http://mli.xylfe.cn

Py:   sorted(arr);  arr.sort()
来源：http://qtt.jinghuilouyu.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://kcb.redwolf501.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://iho.jinqigfzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://cnh.gotoacloud.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://xfs.hnqzz.top

Go:   slices.Sort(arr)
来源：http://nih.hesvh.cn

Ruby: arr.sort
来源：http://frq.pengpengdd.cyou

C#:   Array.Sort(arr);  list.Sort()
来源：http://djk.zycfv.cn

[N03] 快速排序（分治示例）
来源：http://pnq.gogol.net.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fiy.jqgufenzy.top

PHP:  // 递归实现，或用 usort
来源：http://ttb.zhongyouzk.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jmy.sysykeji.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ojp.quarkkingdee.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://lyp.jinghuilouyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://lbt.sxryk.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://eqa.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://ckj.zhoulong.xyz

[N04] 斐波那契数列
来源：http://gbd.yvedp.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://rog.ctjpmb.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://top.cucudq.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sas.aibaodan.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://odw.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pvg.tanke756.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://bxv.meibo888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://jmt.dianchejie.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://eak.fktsv.cn

[N05] 最大公约数
来源：http://dem.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://zts.shangyingyoupin.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://gvc.ywan-chungtsiang.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://mrs.wangdashe.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zup.fehbvm.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://frf.bbcook.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://nct.jqgufenzy.top

Ruby: a.gcd(b)
来源：http://run.gogol.net.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gwq.chenzaomai.com

[N06] 判断回文字符串
来源：http://yuz.guannengcc.top

Py:   s == s[::-1]
来源：http://jdn.hammf.cn

PHP:  $s === strrev($s);
来源：http://prx.fktsv.cn

JS:   s === [...s].reverse().join("")
来源：http://rds.ppjwa.cn

TS:   s === [...s].reverse().join("")
来源：http://ohe.dashuyun.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://qri.ivvv.top

Go:   // 双指针从两端比较
来源：http://fqb.cheryme.top

Ruby: s == s.reverse
来源：http://acf.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ygs.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://ulf.zhijiandao.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lvi.ctjpmb.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://cwt.vqdsnc.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://msj.hesvh.cn

TS:   // 手写 Map<string, number>
来源：http://edh.jianghu66.top

Java: // 手写 HashMap
来源：http://enp.chenlongwang.top

Go:   // 手写 map[int]int
来源：http://ycn.tianlin.xyz

Ruby: // 手写 Hash
来源：http://ynv.fktsv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://mdw.jinqigufen.top

[N08] 生成全排列
来源：http://yxz.jiagoushi.top

Py:   itertools.permutations(arr)
来源：http://jee.vehdjk.com

PHP:  // 手写递归交换
来源：http://zsy.ywan-chungtsiang.top

JS:   // 手写回溯递归
来源：http://nik.zhaomingkeji.xyz

TS:   // 手写回溯递归
来源：http://jin.vehdjk.com

Java: // 手写回溯递归
来源：http://qtl.yueranfly.top

Go:   // 手写回溯递归
来源：http://uko.jianghu66.top

Ruby: arr.permutation.to_a
来源：http://slf.tian-w.cn

C#:   // 手写回溯递归
来源：http://cww.hnqzz.top

[N09] 栈与队列
来源：http://nxy.yvedp.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://oyg.pengpengdd.cyou

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://kfc.guowangkeji.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://avi.iojbl.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://iuu.shzxlz.cn

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://ypi.fktsv.cn

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://rhx.jyoumei.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://gta.zdbjq.cn


<!-- 参考信息 -->