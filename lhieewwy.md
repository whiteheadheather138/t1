代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://qfw.daria6918.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://gnj.hammf.cn

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://qdl.cashguo.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://yeh.yonumen.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://voj.tanke756.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://aue.yuanzhike.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://obf.cheryme.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ksi.kuanghao11.cn

================================================================================
来源：http://xkp.pycfn.com

K. JSON 与序列化
来源：http://bws.cdnleiting.top

================================================================================
来源：http://mdc.guowangkeji.top

[K01] 对象转 JSON 字符串
来源：http://ktq.quarkkingdee.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yif.gzhubu.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://awm.hammf.cn

JS:   JSON.stringify(obj)
来源：http://chg.dianchejie.cn

TS:   JSON.stringify(obj)
来源：http://dht.chenjidiqi.icu

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xxj.kuanghao11.cn

Go:   json.Marshal(obj)
来源：http://buj.ppjwa.cn

Ruby: obj.to_json                                     // require "json"
来源：http://ppe.uphjek.com

C#:   JsonSerializer.Serialize(obj)
来源：http://arw.jinqigufen.top

[K02] JSON 字符串转对象
来源：http://ffd.jinqigfzy.top

Py:   json.loads(s)
来源：http://vmx.hesvh.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kur.xinyue.icu

JS:   JSON.parse(s)
来源：http://lnr.52xcode.cn

TS:   JSON.parse(s)
来源：http://pcq.gogol.net.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vjv.jlsjyb.cn

Go:   json.Unmarshal(data, &v)
来源：http://rdy.zhengqikj.top

Ruby: JSON.parse(s)
来源：http://vfk.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://flg.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://atg.jlsjyb.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://rej.snrcjt.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://neh.daxiang520.top

JS:   JSON.stringify(obj, null, 2)
来源：http://xre.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://zyk.bbcook.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://qnn.dashuyun.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://bdc.gaohongyu789.top

Ruby: JSON.pretty_generate(obj)
来源：http://oiv.ywan-chungtsiang.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://icr.meibo888.top

[K04] 读取 JSON 文件
来源：http://quh.yuanzhike.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://kps.yuanzhike.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cli.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://atg.dashuyun.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://atp.ywan-chungtsiang.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mfg.shanyushiyangkeji.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://fmh.andypj.xyz

Ruby: JSON.parse(File.read("a.json"))
来源：http://ftf.jlsjyb.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://jcr.hesvh.cn

[K05] 深拷贝对象
来源：http://ofi.feifeiyinyue.top

Py:   copy.deepcopy(obj)
来源：http://ref.tianlin.xyz

PHP:  unserialize(serialize($obj));
来源：http://hzg.aibaodan.cn

JS:   structuredClone(obj)
来源：http://yas.ehwqpu.com

TS:   structuredClone(obj)
来源：http://xya.fengsongda.top

Java: // 手写拷贝构造，或序列化往返
来源：http://jed.ybcxt.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://cpw.vehdjk.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://uey.jinyuanbaomall.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://pog.zycfv.cn

[K06] 解析 URL 查询串
来源：http://vsd.chenlongwang.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://hnz.zhixingplan.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vmo.gaohongyu789.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://siv.yueranfly.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ppx.gotoacloud.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ebu.ydzc1.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://efk.tian-w.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://uas.quarkkingdee.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://wzl.hysaishi.cn

[K07] 进制转换
来源：http://izz.sxryk.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bik.jqgfzy.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://znk.xinyue.icu

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://dmo.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://aeu.gotoacloud.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://rmq.redwolf501.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xts.sweek.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://hcf.pengpengdd.cyou

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fao.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://xfi.jinghuilouyu.cn

Py:   pickle.dumps(obj)
来源：http://saa.ydjk.org.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://gbx.bjfxy.top

JS:   v8.serialize(obj)        // Node
来源：http://axi.316326.xyz

TS:   v8.serialize(obj)        // Node
来源：http://xlg.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://ztw.yonumen.top

Go:   encoding/gob
来源：http://ljd.ehwqpu.com

Ruby: Marshal.dump(obj)
来源：http://nin.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://sdw.sxryk.cn

================================================================================
来源：http://wuj.tanke756.top

L. 网络请求
来源：http://isb.jianghu66.top

================================================================================
来源：http://tfx.smart0.xyz

[L01] 发送 GET 请求
来源：http://nvv.hfpthk.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://pwm.nwbrower.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://agl.jinqigufen.top

JS:   await fetch(url)
来源：http://zdq.gotoacloud.top

TS:   await fetch(url)
来源：http://flo.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://egl.jianghu66.top

Go:   resp, err := http.Get(url)
来源：http://vwj.haohaochexian.top

Ruby: Net::HTTP.get(URI(url))
来源：http://wje.shuidangran.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dit.zhiwuduotai.top

[L02] 发送 POST JSON
来源：http://fnc.aibaodan.cn

Py:   requests.post(url, json={"a": 1})
来源：http://hfj.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gux.dianchejie.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cdj.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://whe.mhx1999.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://exw.0kj1m.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fqe.gogol.net.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://ntt.tian-w.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bet.nanxinkj.top

[L03] 设置自定义请求头
来源：http://fsf.shangyingyoupin.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://jvd.cheryme.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://qau.xylfe.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://oyr.ehwqpu.com

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zli.sweek.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://kqk.sufxvd.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gpk.wangdashe.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eya.tanke756.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://fwy.cdnleiting.top

[L04] 设置超时
来源：http://zih.hysaishi.cn

Py:   requests.get(url, timeout=5)
来源：http://gyh.sjlbkw.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://quw.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://edn.hnqzz.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zox.xziqi.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://zol.tian-w.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://yrn.zhixingplan.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mjv.aizwys.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://joz.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://gcj.yj20258888.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://phq.ybcxt.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://tqe.jinqigfzy.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://brg.zhongyouzk.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://exg.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://gvc.dashuyun.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://tgw.xziqi.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://egp.52xcode.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://krw.daxiang520.top

[L06] 解析响应为 JSON
来源：http://utc.fktsv.cn

Py:   resp.json()
来源：http://lww.cheryme.top

PHP:  json_decode($body, true);
来源：http://ujw.guannengcc.top

JS:   await resp.json()
来源：http://dgh.uphjek.com

TS:   await resp.json()
来源：http://gfq.gzhubu.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xin.yvedp.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://ncq.cqqwz.cn

Ruby: JSON.parse(resp.body)
来源：http://gaf.ctjpmb.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ehm.haohaochexian.top

[L07] 处理 HTTP 状态码
来源：http://djb.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://cjr.shuidangran.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://pva.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://eau.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://doh.xylfe.cn

Java: resp.statusCode()
来源：http://egl.ppjwa.cn

Go:   resp.StatusCode
来源：http://meh.gaohongyu789.top

Ruby: resp.code.to_i
来源：http://etm.hnqzz.top

C#:   (int)resp.StatusCode
来源：http://fte.shangyingyoupin.top

[L08] 并发请求多个地址
来源：http://gek.xuanzx.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nkt.andypj.xyz

PHP:  curl_multi_init() 系列
来源：http://klv.jinqigfzy.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ngc.feifeiyinyue.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qyo.xuetiantiany.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://jou.c1oappe.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ixu.gotoacloud.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://stx.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fim.yj202588.top

================================================================================
来源：http://djj.sweek.top

M. 命令行 / 进程 / 环境
来源：http://iku.zhengqikj.top

================================================================================
来源：http://ank.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://qwj.guannengcc.top

Py:   sys.argv[1:]
来源：http://yvd.yuxming.cn

PHP:  $argv;  $argc;
来源：http://sxz.52xcode.cn

JS:   process.argv.slice(2)
来源：http://jeo.svipenyu.cn

TS:   process.argv.slice(2)
来源：http://zmc.yfazqb.com

Java: args 数组（main 方法参数）
来源：http://wcg.jlsjyb.cn

Go:   os.Args[1:]
来源：http://jil.cashguo.top

Ruby: ARGV
来源：http://jez.andypj.xyz

C#:   args 数组（Main 方法参数）
来源：http://kyr.yj202588.top

[M02] 读取环境变量
来源：http://vnm.zhiwuduotai.top

Py:   os.environ.get("HOME")
来源：http://ana.yueranfly.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tvc.hcnkem.com

JS:   process.env.HOME
来源：http://xej.pengpengdd.cyou

TS:   process.env.HOME
来源：http://vni.guowangkeji.top

Java: System.getenv("HOME")
来源：http://ael.tian-w.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://vmu.yj202588.top

Ruby: ENV["HOME"]
来源：http://xro.sxryk.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nda.guowangkeji.top

[M03] 执行外部命令
来源：http://xys.hnqzz.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://rye.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://qtm.uphjek.com

JS:   child_process.execSync("ls -l").toString()
来源：http://uyw.tanke756.top

TS:   child_process.execSync("ls -l").toString()
来源：http://afk.tarul.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://jxh.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://uri.xuetiantiany.cn

Ruby: system("ls -l");  `ls -l`
来源：http://sop.hnqzz.top

C#:   Process.Start("ls", "-l");
来源：http://whn.shanyushiyangtech.top

[M04] 获取当前工作目录
来源：http://ccx.sweek.top

Py:   os.getcwd()
来源：http://igq.sjlbkw.cn

PHP:  getcwd();
来源：http://vzk.daria6918.cn

JS:   process.cwd()
来源：http://abk.zhiwuduotai.top

TS:   process.cwd()
来源：http://xai.jinqigfzy.top

Java: Path.of("").toAbsolutePath()
来源：http://ler.0kj1m.cn

Go:   os.Getwd()
来源：http://olu.svipenyu.cn

Ruby: Dir.pwd
来源：http://ztm.iojbl.cn

C#:   Directory.GetCurrentDirectory()
来源：http://wpt.uphjek.com

[M05] 设置退出码
来源：http://sru.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://fiz.zycfv.cn

PHP:  exit(1);
来源：http://btx.hammf.cn

JS:   process.exit(1)
来源：http://nxs.dashuyun.cn

TS:   process.exit(1)
来源：http://cgj.sysykeji.top

Java: System.exit(1)
来源：http://dct.fanxiaobao.xyz

Go:   os.Exit(1)
来源：http://vev.jinqigfzy.top

Ruby: exit 1
来源：http://fjn.tian-w.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://xtx.guowangkeji.top

[M06] 向标准错误输出
来源：http://amp.nwbrower.top

Py:   print("err", file=sys.stderr)
来源：http://jub.yuanzhike.top

PHP:  fwrite(STDERR, "err\n");
来源：http://qic.xziqi.cn

JS:   console.error("err")
来源：http://czr.gzhubu.top

TS:   console.error("err")
来源：http://wlf.aibaodan.cn

Java: System.err.println("err")
来源：http://mox.xziqi.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ciq.aibaodan.cn

Ruby: warn "err"
来源：http://bul.mhx1999.top

C#:   Console.Error.WriteLine("err")
来源：http://jdf.vehdjk.com

[M07] 判断是否为主入口
来源：http://xfw.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://gwi.hnxiangtu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://wjg.zhongyouzk.top

JS:   require.main === module
来源：http://srw.tian-w.cn

TS:   require.main === module
来源：http://lgt.uphjek.com

Java: public static void main(String[] args)
来源：http://uwm.ivvv.top

Go:   func main()
来源：http://jde.jinghuilouyu.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://csb.nanxuanxn.top

C#:   static void Main(string[] args)
来源：http://jcc.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://kzt.jlsjyb.cn

Py:   platform.system();  platform.python_version()
来源：http://fra.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://zbz.tian-w.cn

JS:   process.platform;  process.version
来源：http://zlv.shzxlz.cn

TS:   process.platform;  process.version
来源：http://omz.ywan-chungtsiang.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ixn.cucudq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ged.ydjk.org.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://jzh.epnwcf.com

C#:   Environment.OSVersion;  Environment.Version
来源：http://yhe.zycfv.cn

================================================================================
来源：http://drr.zdbjq.cn

N. 数据结构与算法
来源：http://fzl.316326.xyz

================================================================================
来源：http://glq.ydzc1.top

[N01] 二分查找（有序数组）
来源：http://nwr.jiagoushi.top

Py:   bisect.bisect_left(arr, x)
来源：http://hlt.nanxinkj.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pkl.hammf.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eqg.iojbl.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hbv.yueranfly.top

Java: Arrays.binarySearch(arr, x)
来源：http://ufu.snrcjt.cn

Go:   sort.SearchInts(arr, x)
来源：http://qyc.shanyushiyangtech.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://owp.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://ipo.jiagoushi.top

[N02] 排序（工程实践用内置实现）
来源：http://iwz.jlsjyb.cn

Py:   sorted(arr);  arr.sort()
来源：http://olg.52xcode.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gkz.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://vsr.hesvh.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://jqj.ydjk.org.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://arr.ctjpmb.com

Go:   slices.Sort(arr)
来源：http://kkv.guannengcc.top

Ruby: arr.sort
来源：http://erw.xylfe.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://lku.ydzc1.top

[N03] 快速排序（分治示例）
来源：http://nhu.guannengcc.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tki.jinqigufen.top

PHP:  // 递归实现，或用 usort
来源：http://omf.yj20258.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vem.daxiang520.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iho.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hpg.pycfn.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vei.ywan-chungtsiang.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rjm.kuanghao11.cn

C#:   // 手写递归，或 Array.Sort
来源：http://vxr.guowangkeji.top

[N04] 斐波那契数列
来源：http://hhg.yonumen.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nxi.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gxa.chenjidiqi.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://iyr.gogol.net.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wst.zhongyouzk.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yqr.nanxinkj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://acf.jlsjyb.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://zjd.jinqigfzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://awp.cdnleiting.top

[N05] 最大公约数
来源：http://xng.havefunace.top

Py:   math.gcd(a, b)
来源：http://aus.kuanghao11.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mdn.pengpengdd.cyou

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://pym.jiagoushi.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://wtw.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rcy.chenlongwang.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://gzw.cashguo.top

Ruby: a.gcd(b)
来源：http://oux.zhiwuduotai.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://oqm.ppjwa.cn

[N06] 判断回文字符串
来源：http://bae.chenlongwang.top

Py:   s == s[::-1]
来源：http://ejw.fengsongda.top

PHP:  $s === strrev($s);
来源：http://mxc.dianchejie.cn

JS:   s === [...s].reverse().join("")
来源：http://tsl.nanxinkj.top

TS:   s === [...s].reverse().join("")
来源：http://bgy.ivvv.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wcz.ivvv.top

Go:   // 双指针从两端比较
来源：http://hyt.hnxiangtu.top

Ruby: s == s.reverse
来源：http://yjq.cashguo.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://hbj.mhx1999.top

[N07] 两数之和（返回下标）
来源：http://gmv.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://hjb.jinqigufen.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://zqh.fktsv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://fsr.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://pct.sweek.top

Java: // 手写 HashMap
来源：http://qja.gogol.net.cn

Go:   // 手写 map[int]int
来源：http://iwr.yongpay.top

Ruby: // 手写 Hash
来源：http://cgn.yangfankeji.com

C#:   // 手写 Dictionary<int, int>
来源：http://wur.aizwys.cn

[N08] 生成全排列
来源：http://mdv.ydjk.org.cn


<!-- 参考信息 -->