代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dgj.cheryme.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://obl.smart0.xyz

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://xqb.jinyuanbaomall.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://wsz.cheryme.top

================================================================================
来源：http://chc.hongshengwenyu.top

K. JSON 与序列化
来源：http://chc.hcnkem.com

================================================================================
来源：http://urg.aizwys.cn

[K01] 对象转 JSON 字符串
来源：http://epx.xinyue.icu

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://owj.shzxlz.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://voj.yj20258.top

JS:   JSON.stringify(obj)
来源：http://uvo.zhengqikj.top

TS:   JSON.stringify(obj)
来源：http://psq.hcnkem.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://kut.guannengcc.top

Go:   json.Marshal(obj)
来源：http://efv.andypj.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://mba.gogol.net.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://flf.yuxming.cn

[K02] JSON 字符串转对象
来源：http://oid.jlsjyb.cn

Py:   json.loads(s)
来源：http://qki.hnxiangtu.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://mqd.ppjwa.cn

JS:   JSON.parse(s)
来源：http://ora.epnwcf.com

TS:   JSON.parse(s)
来源：http://nyl.epnwcf.com

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://xws.snrcjt.cn

Go:   json.Unmarshal(data, &v)
来源：http://fxf.yueranfly.top

Ruby: JSON.parse(s)
来源：http://pue.dianchejie.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jgf.dianchejie.cn

[K03] JSON 美化输出（带缩进）
来源：http://mpt.ctjpmb.com

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://nnc.shzxlz.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://xka.yvedp.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://pfw.52xcode.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://djb.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lln.gzhubu.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://zhc.9152youxi.cn

Ruby: JSON.pretty_generate(obj)
来源：http://dtx.jlsjyb.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jdc.guannengcc.top

[K04] 读取 JSON 文件
来源：http://laf.cqqwz.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xmm.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xmy.316326.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://mee.jianghu66.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aqy.daxiang520.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://ctc.smart0.xyz

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://sep.redwolf501.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://yyk.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://est.jinyuanbaomall.cn

[K05] 深拷贝对象
来源：http://mnt.jqgfzy.top

Py:   copy.deepcopy(obj)
来源：http://ctg.ydzc1.top

PHP:  unserialize(serialize($obj));
来源：http://wxx.yfazqb.com

JS:   structuredClone(obj)
来源：http://vbn.ydzc1.top

TS:   structuredClone(obj)
来源：http://zwv.iojbl.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://uuv.9152youxi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://msj.haohaochexian.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://gah.chenlongwang.top

C#:   // 序列化往返，或自定义 Clone
来源：http://wkb.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://kqq.xinyue.icu

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://svp.andypj.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://nud.chenlongwang.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mnr.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uyc.pycfn.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://jxp.fengsongda.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://rhq.sweek.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fmv.hnxiangtu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://yao.zhoulong.xyz

[K07] 进制转换
来源：http://xde.hnqzz.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://sgo.sufxvd.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://beq.chenlongwang.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://txz.sxryk.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://myj.gogol.net.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bty.redwolf501.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lyn.kuanghao11.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://gtr.gogol.net.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mhx.jqgfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://rnh.bjfxy.top

Py:   pickle.dumps(obj)
来源：http://sqf.cashguo.top

PHP:  serialize($obj);  unserialize($s);
来源：http://nnj.yuanzhike.top

JS:   v8.serialize(obj)        // Node
来源：http://kdq.smart0.xyz

TS:   v8.serialize(obj)        // Node
来源：http://ujq.ywan-chungtsiang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cig.zycfv.cn

Go:   encoding/gob
来源：http://vbw.9152youxi.cn

Ruby: Marshal.dump(obj)
来源：http://nam.hnqzz.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://aiq.fktsv.cn

================================================================================
来源：http://fwk.yueranfly.top

L. 网络请求
来源：http://ugf.cashguo.top

================================================================================
来源：http://ope.gzhubu.top

[L01] 发送 GET 请求
来源：http://vgo.guannengcc.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dqe.yj20258888.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://exd.shuidangran.top

JS:   await fetch(url)
来源：http://tct.redwolf501.top

TS:   await fetch(url)
来源：http://svy.guowangkeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ade.sufxvd.cn

Go:   resp, err := http.Get(url)
来源：http://fto.gotoacloud.top

Ruby: Net::HTTP.get(URI(url))
来源：http://jub.yj20258.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wpu.wangdashe.top

[L02] 发送 POST JSON
来源：http://cox.nanxuanxn.top

Py:   requests.post(url, json={"a": 1})
来源：http://bay.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rxv.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rlk.gotoacloud.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tvb.tanke756.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://qrs.jlsjyb.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://nlj.bjfxy.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vnd.epnwcf.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://dhn.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://vcl.yongpay.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zum.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://jpo.ctjpmb.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://dob.hesvh.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://urg.ydjk.org.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gqb.hfpthk.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gqz.gzhubu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dlf.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://qhq.xingfuxueyuan.xyz

[L04] 设置超时
来源：http://hel.zdqjudy.top

Py:   requests.get(url, timeout=5)
来源：http://tds.hongshengwenyu.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://fjd.hfpthk.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://kpm.smart0.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://axn.cqqwz.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://eph.tarul.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://lwh.yonumen.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://khg.cashguo.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://yey.shangyingyoupin.top

[L05] 上传文件（multipart）
来源：http://zhc.yuanzhike.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://zyo.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ols.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://dzh.tianlin.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jhh.snrcjt.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ync.yuanzhike.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://jhr.haohaochexian.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://ltn.hammf.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dnz.gaohongyu789.top

[L06] 解析响应为 JSON
来源：http://wsw.vqdsnc.cn

Py:   resp.json()
来源：http://mxh.guowangkeji.top

PHP:  json_decode($body, true);
来源：http://hpm.yj20258888.top

JS:   await resp.json()
来源：http://pnj.shangyingyoupin.top

TS:   await resp.json()
来源：http://jnu.cqqwz.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xly.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vqh.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://spq.uphjek.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mkz.daxiang520.top

[L07] 处理 HTTP 状态码
来源：http://ttn.havefunace.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://bxj.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nhg.hywenlv.cn

JS:   resp.ok;  resp.status
来源：http://hgy.yangfankeji.com

TS:   resp.ok;  resp.status
来源：http://gkt.uphjek.com

Java: resp.statusCode()
来源：http://ouo.bbcook.cn

Go:   resp.StatusCode
来源：http://ygs.zycfv.cn

Ruby: resp.code.to_i
来源：http://iwc.gotoacloud.top

C#:   (int)resp.StatusCode
来源：http://yyv.ctjpmb.com

[L08] 并发请求多个地址
来源：http://srq.yfazqb.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ssd.epnwcf.com

PHP:  curl_multi_init() 系列
来源：http://cux.sufxvd.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://spn.meibo888.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nlz.sweek.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lcl.zhiwuduotai.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://fka.tian-w.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://sxl.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://sfx.ivvv.top

================================================================================
来源：http://ino.hnqzz.top

M. 命令行 / 进程 / 环境
来源：http://gjt.ywan-chungtsiang.top

================================================================================
来源：http://vmt.hammf.cn

[M01] 读取命令行参数
来源：http://gvl.pycfn.com

Py:   sys.argv[1:]
来源：http://tnb.daria6918.cn

PHP:  $argv;  $argc;
来源：http://feq.jqgufenzy.top

JS:   process.argv.slice(2)
来源：http://wka.redwolf501.top

TS:   process.argv.slice(2)
来源：http://hcp.c1oappe.top

Java: args 数组（main 方法参数）
来源：http://qeg.yj20258.top

Go:   os.Args[1:]
来源：http://sor.xinyue.icu

Ruby: ARGV
来源：http://cln.xinyue.icu

C#:   args 数组（Main 方法参数）
来源：http://ruo.tanke756.top

[M02] 读取环境变量
来源：http://jhs.meibo888.top

Py:   os.environ.get("HOME")
来源：http://ypv.jqgufenzy.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://wrw.redwolf501.top

JS:   process.env.HOME
来源：http://mzr.jinyuanbaomall.cn

TS:   process.env.HOME
来源：http://osp.epnwcf.com

Java: System.getenv("HOME")
来源：http://foq.hfpthk.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://pvd.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://fcl.yuanzhike.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://vgf.jiagoushi.top

[M03] 执行外部命令
来源：http://wxo.hysaishi.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ehf.quarkkingdee.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kwx.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://zde.snrcjt.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rdw.yuanzhike.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://lhn.daxiang520.top

Go:   exec.Command("ls", "-l").Output()
来源：http://ucz.jlsjyb.cn

Ruby: system("ls -l");  `ls -l`
来源：http://mit.bbcook.cn

C#:   Process.Start("ls", "-l");
来源：http://zti.shangyingyoupin.top

[M04] 获取当前工作目录
来源：http://xaz.sysykeji.top

Py:   os.getcwd()
来源：http://hpt.mhx1999.top

PHP:  getcwd();
来源：http://ear.9152youxi.cn

JS:   process.cwd()
来源：http://hrp.ybcxt.top

TS:   process.cwd()
来源：http://tax.hammf.cn

Java: Path.of("").toAbsolutePath()
来源：http://vjw.yonumen.top

Go:   os.Getwd()
来源：http://bcj.shanyushiyangtech.top

Ruby: Dir.pwd
来源：http://pyj.jinyuanbaomall.cn

C#:   Directory.GetCurrentDirectory()
来源：http://oty.hnxiangtu.top

[M05] 设置退出码
来源：http://dtm.smart0.xyz

Py:   sys.exit(1)
来源：http://qny.birdmap.top

PHP:  exit(1);
来源：http://rcl.jqgfzy.top

JS:   process.exit(1)
来源：http://nfp.hesvh.cn

TS:   process.exit(1)
来源：http://rfs.cashguo.top

Java: System.exit(1)
来源：http://tzn.jinghuilouyu.cn

Go:   os.Exit(1)
来源：http://gkr.xinyue.icu

Ruby: exit 1
来源：http://nkz.haohaochexian.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vmc.aibaodan.cn

[M06] 向标准错误输出
来源：http://kpn.zhengqikj.top

Py:   print("err", file=sys.stderr)
来源：http://msu.9152youxi.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://tma.jinqigfzy.top

JS:   console.error("err")
来源：http://jvi.zdbjq.cn

TS:   console.error("err")
来源：http://vfd.yangfankeji.com

Java: System.err.println("err")
来源：http://bxn.feifeiyinyue.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ikp.yfazqb.com

Ruby: warn "err"
来源：http://alq.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://ohp.yj20258888.top

[M07] 判断是否为主入口
来源：http://fay.haohaochexian.top

Py:   if __name__ == "__main__":
来源：http://vin.nwbrower.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://blm.kuanghao11.cn

JS:   require.main === module
来源：http://jtv.wangshuangyany.cn

TS:   require.main === module
来源：http://eoq.yfazqb.com

Java: public static void main(String[] args)
来源：http://brn.shanyushiyangkeji.top

Go:   func main()
来源：http://amq.vqdsnc.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://vyz.jqgfzy.top

C#:   static void Main(string[] args)
来源：http://zkh.sweek.top

[M08] 获取系统与运行时信息
来源：http://jpp.hesvh.cn

Py:   platform.system();  platform.python_version()
来源：http://nsh.snrcjt.cn

PHP:  PHP_OS;  phpversion();
来源：http://fas.9152youxi.cn

JS:   process.platform;  process.version
来源：http://qnf.dashuyun.cn

TS:   process.platform;  process.version
来源：http://his.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://mdf.sjlbkw.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jsl.yfazqb.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://feu.smart0.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://hiv.jqgfzy.top

================================================================================
来源：http://hfi.jinghuilouyu.cn

N. 数据结构与算法
来源：http://nri.shzxlz.cn

================================================================================
来源：http://sko.uphjek.com

[N01] 二分查找（有序数组）
来源：http://eto.nanxuanxn.top

Py:   bisect.bisect_left(arr, x)
来源：http://mnx.zhijiandao.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://jvc.jiagoushi.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://icc.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://lef.tian-w.cn

Java: Arrays.binarySearch(arr, x)
来源：http://dsv.tian-w.cn

Go:   sort.SearchInts(arr, x)
来源：http://ffb.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://pku.dashuyun.cn

C#:   Array.BinarySearch(arr, x)
来源：http://bbb.fehbvm.com

[N02] 排序（工程实践用内置实现）
来源：http://hpw.hfpthk.cn

Py:   sorted(arr);  arr.sort()
来源：http://mdh.hcnkem.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://bji.hongshengwenyu.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://mrm.hongshengwenyu.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ufz.pycfn.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://nbf.mhx1999.top

Go:   slices.Sort(arr)
来源：http://hjo.yanxiufei.cn

Ruby: arr.sort
来源：http://uje.jianghu66.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yes.ywan-chungtsiang.top

[N03] 快速排序（分治示例）
来源：http://azv.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://wft.daria6918.cn

PHP:  // 递归实现，或用 usort
来源：http://jny.meibo888.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yqg.xuanzx.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://xay.ehwqpu.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://stp.jianghu66.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kbn.xuetiantiany.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://gdy.bjfxy.top

C#:   // 手写递归，或 Array.Sort
来源：http://fxj.dianchejie.cn

[N04] 斐波那契数列
来源：http://fom.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://whc.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ygt.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bdj.zhiwuduotai.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://cgq.jianghu66.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://fpy.cucudq.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://sft.shanyushiyangtech.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zls.pengpengdd.cyou

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://hwg.pycfn.com

[N05] 最大公约数
来源：http://cuz.zhaomingkeji.xyz

Py:   math.gcd(a, b)
来源：http://lyo.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pct.yvedp.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lio.fehbvm.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ctm.gogol.net.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://cvs.dianchejie.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qas.nwbrower.top

Ruby: a.gcd(b)
来源：http://zyi.wangshuangyany.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ewr.ywan-chungtsiang.top

[N06] 判断回文字符串
来源：http://bjv.zhengqikj.top

Py:   s == s[::-1]
来源：http://bvk.sufxvd.cn

PHP:  $s === strrev($s);
来源：http://tbs.yuxming.cn

JS:   s === [...s].reverse().join("")
来源：http://fap.cdnleiting.top

TS:   s === [...s].reverse().join("")
来源：http://fhi.fktsv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ivb.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://dcf.shangyingyoupin.top

Ruby: s == s.reverse
来源：http://sii.redwolf501.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://igb.gzhubu.top

[N07] 两数之和（返回下标）
来源：http://rgu.vqdsnc.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://zos.ydjk.org.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://orl.dashuyun.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cqn.xziqi.cn

TS:   // 手写 Map<string, number>
来源：http://nma.fehbvm.com

Java: // 手写 HashMap
来源：http://jqf.ydzc1.top

Go:   // 手写 map[int]int
来源：http://owy.hongshengwenyu.top

Ruby: // 手写 Hash
来源：http://sgb.jinyuanbaomall.cn

C#:   // 手写 Dictionary<int, int>
来源：http://erz.sweek.top

[N08] 生成全排列
来源：http://rec.fanxiaobao.xyz

Py:   itertools.permutations(arr)
来源：http://tbj.guowangkeji.top

PHP:  // 手写递归交换
来源：http://nrb.uphjek.com

JS:   // 手写回溯递归
来源：http://vyh.bbcook.cn

TS:   // 手写回溯递归
来源：http://apw.daria6918.cn


<!-- 参考信息 -->