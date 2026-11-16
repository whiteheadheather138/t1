代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://lne.zhongyouzk.top

Ruby: Time.now.getlocal("+08:00")
来源：http://rid.jyoumei.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://eqx.redwolf501.top

[J10] 取今天 / 本月第一天
来源：http://gaa.zdbjq.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://clt.yfazqb.com

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://cyq.yj202588.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://hie.epnwcf.com

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://ewh.zdbjq.cn

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://eda.chenjidiqi.icu

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lsn.chenjidiqi.icu

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rjs.0kj1m.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nnm.zdbjq.cn

================================================================================
来源：http://ipe.xziqi.cn

K. JSON 与序列化
来源：http://rqo.vehdjk.com

================================================================================
来源：http://hkl.sweek.top

[K01] 对象转 JSON 字符串
来源：http://lrj.yuanzhike.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wjd.snrcjt.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://ner.zhixingplan.top

JS:   JSON.stringify(obj)
来源：http://oeg.smart0.xyz

TS:   JSON.stringify(obj)
来源：http://dpf.ywan-chungtsiang.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://cug.iojbl.cn

Go:   json.Marshal(obj)
来源：http://uxn.yueranfly.top

Ruby: obj.to_json                                     // require "json"
来源：http://ome.birdmap.top

C#:   JsonSerializer.Serialize(obj)
来源：http://qij.316326.xyz

[K02] JSON 字符串转对象
来源：http://ezg.tanke756.top

Py:   json.loads(s)
来源：http://yjb.ivvv.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://jqy.shuidangran.top

JS:   JSON.parse(s)
来源：http://qdm.vqdsnc.cn

TS:   JSON.parse(s)
来源：http://onh.sufxvd.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://arb.meibo888.top

Go:   json.Unmarshal(data, &v)
来源：http://wjw.dianchejie.cn

Ruby: JSON.parse(s)
来源：http://kqa.aibaodan.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://bnp.andypj.xyz

[K03] JSON 美化输出（带缩进）
来源：http://xyx.jinghuilouyu.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://ikf.sysykeji.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://kwi.yueranfly.top

JS:   JSON.stringify(obj, null, 2)
来源：http://aui.gotoacloud.top

TS:   JSON.stringify(obj, null, 2)
来源：http://apl.xingfuxueyuan.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iwc.fehbvm.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gfd.hnxiangtu.top

Ruby: JSON.pretty_generate(obj)
来源：http://yof.shzxlz.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tdi.jinqigfzy.top

[K04] 读取 JSON 文件
来源：http://jvy.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://uyi.jinqigfzy.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cxe.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://sqf.hcnkem.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zat.yj202588.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://jlf.9152youxi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://htq.wangdashe.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://fbf.hnxiangtu.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://gzq.fanxiaobao.xyz

[K05] 深拷贝对象
来源：http://asr.yueranfly.top

Py:   copy.deepcopy(obj)
来源：http://kbs.jianghu66.top

PHP:  unserialize(serialize($obj));
来源：http://vng.smart0.xyz

JS:   structuredClone(obj)
来源：http://jih.hnqzz.top

TS:   structuredClone(obj)
来源：http://nfn.kuanghao11.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://vsf.fktsv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fqi.hywenlv.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://jhb.havefunace.top

C#:   // 序列化往返，或自定义 Clone
来源：http://mpu.sweek.top

[K06] 解析 URL 查询串
来源：http://eys.ydzc1.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ogp.cucudq.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://kdq.hysaishi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gsu.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yxj.hfpthk.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://xya.tian-w.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://qds.sufxvd.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zow.jyoumei.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zvg.ydjk.org.cn

[K07] 进制转换
来源：http://hot.xziqi.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://gxi.hammf.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://mkq.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bov.uphjek.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tsv.ctjpmb.com

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://oky.wangshuangyany.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://xve.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kuk.ivvv.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://wmb.fengsongda.top

[K08] 二进制序列化（非 JSON）
来源：http://alm.cashguo.top

Py:   pickle.dumps(obj)
来源：http://yzp.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pkd.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://yfu.gogol.net.cn

TS:   v8.serialize(obj)        // Node
来源：http://vzs.hfpthk.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://uca.xylfe.cn

Go:   encoding/gob
来源：http://zgf.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://ifa.fehbvm.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jbw.hysaishi.cn

================================================================================
来源：http://obn.xingfuxueyuan.xyz

L. 网络请求
来源：http://ulx.cdnleiting.top

================================================================================
来源：http://cks.chenzaomai.com

[L01] 发送 GET 请求
来源：http://cdg.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rgf.gogol.net.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://jql.cheryme.top

JS:   await fetch(url)
来源：http://ijc.xziqi.cn

TS:   await fetch(url)
来源：http://gmc.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://qiw.hcnkem.com

Go:   resp, err := http.Get(url)
来源：http://lpw.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://wsf.svipenyu.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://nzs.hnxiangtu.top

[L02] 发送 POST JSON
来源：http://tdf.316326.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://pzx.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://nni.wangdashe.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://vnd.xylfe.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://ksh.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://tog.shanyushiyangkeji.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://dfh.xylfe.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://jlc.ybcxt.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nef.9152youxi.cn

[L03] 设置自定义请求头
来源：http://ebo.fktsv.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://udc.nanxinkj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ssf.aizwys.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fjg.birdmap.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://git.aizwys.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://wty.redwolf501.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://wht.yuxming.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://fsl.yfazqb.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mbu.sjlbkw.cn

[L04] 设置超时
来源：http://jjn.uphjek.com

Py:   requests.get(url, timeout=5)
来源：http://tsy.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://duy.pengpengdd.cyou

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://fdt.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://gvl.pycfn.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://szc.shangyingyoupin.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xad.sweek.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://jzo.hysaishi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mtt.ydzc1.top

[L05] 上传文件（multipart）
来源：http://wwv.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://oxk.c1oappe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ufn.svipenyu.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qoi.pengpengdd.cyou

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://seh.pycfn.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://guv.daxiang520.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ajf.yongpay.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fcd.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://lvd.nanxinkj.top

[L06] 解析响应为 JSON
来源：http://fxn.pengpengdd.cyou

Py:   resp.json()
来源：http://cyk.zhaomingkeji.xyz

PHP:  json_decode($body, true);
来源：http://lbq.cheryme.top

JS:   await resp.json()
来源：http://fyr.jinqigufen.top

TS:   await resp.json()
来源：http://jwt.yueranfly.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://fzz.sysykeji.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pdt.ybcxt.top

Ruby: JSON.parse(resp.body)
来源：http://qrw.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://jmt.nanxinkj.top

[L07] 处理 HTTP 状态码
来源：http://mao.svipenyu.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ppu.zdqjudy.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ztv.zhengqikj.top

JS:   resp.ok;  resp.status
来源：http://zvi.shuidangran.top

TS:   resp.ok;  resp.status
来源：http://eeq.bbcook.cn

Java: resp.statusCode()
来源：http://try.dianchejie.cn

Go:   resp.StatusCode
来源：http://tkr.fengsongda.top

Ruby: resp.code.to_i
来源：http://xsy.jqgufenzy.top

C#:   (int)resp.StatusCode
来源：http://rre.meibo888.top

[L08] 并发请求多个地址
来源：http://lst.sxryk.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://nmo.tarul.cn

PHP:  curl_multi_init() 系列
来源：http://xdc.bbcook.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://nuw.shangyingyoupin.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vkp.9152youxi.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://scr.ppjwa.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://jbf.zdqjudy.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ibx.zhiwuduotai.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://asy.yj202588.top

================================================================================
来源：http://xuk.gogol.net.cn

M. 命令行 / 进程 / 环境
来源：http://txv.zhijiandao.cn

================================================================================
来源：http://twk.hongshengwenyu.top

[M01] 读取命令行参数
来源：http://ycf.bjfxy.top

Py:   sys.argv[1:]
来源：http://mua.sxryk.cn

PHP:  $argv;  $argc;
来源：http://jwi.smart0.xyz

JS:   process.argv.slice(2)
来源：http://bqn.zhengqikj.top

TS:   process.argv.slice(2)
来源：http://leq.sysykeji.top

Java: args 数组（main 方法参数）
来源：http://mey.xingfuxueyuan.xyz

Go:   os.Args[1:]
来源：http://xnt.yj20258888.top

Ruby: ARGV
来源：http://zdx.316326.xyz

C#:   args 数组（Main 方法参数）
来源：http://ktw.cashguo.top

[M02] 读取环境变量
来源：http://wts.yongpay.top

Py:   os.environ.get("HOME")
来源：http://ywb.dianchejie.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://cht.nwbrower.top

JS:   process.env.HOME
来源：http://ggp.pycfn.com

TS:   process.env.HOME
来源：http://rgk.zhaomingkeji.xyz

Java: System.getenv("HOME")
来源：http://zqf.xuanzx.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://svo.guowangkeji.top

Ruby: ENV["HOME"]
来源：http://aej.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fke.svipenyu.cn

[M03] 执行外部命令
来源：http://ngv.sxryk.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://nvt.9152youxi.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://bja.smart0.xyz

JS:   child_process.execSync("ls -l").toString()
来源：http://byj.hongshengwenyu.top

TS:   child_process.execSync("ls -l").toString()
来源：http://bko.nwbrower.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eot.nwbrower.top

Go:   exec.Command("ls", "-l").Output()
来源：http://env.pengpengdd.cyou

Ruby: system("ls -l");  `ls -l`
来源：http://kiv.yuxming.cn

C#:   Process.Start("ls", "-l");
来源：http://mmh.hysaishi.cn

[M04] 获取当前工作目录
来源：http://xtp.bjfxy.top

Py:   os.getcwd()
来源：http://mai.xziqi.cn

PHP:  getcwd();
来源：http://jih.tianlin.xyz

JS:   process.cwd()
来源：http://fpl.ybcxt.top

TS:   process.cwd()
来源：http://duf.mhx1999.top

Java: Path.of("").toAbsolutePath()
来源：http://nyc.gaohongyu789.top

Go:   os.Getwd()
来源：http://hqo.ctjpmb.com

Ruby: Dir.pwd
来源：http://qbs.tian-w.cn

C#:   Directory.GetCurrentDirectory()
来源：http://znp.redwolf501.top

[M05] 设置退出码
来源：http://vqg.shzxlz.cn

Py:   sys.exit(1)
来源：http://ghu.vehdjk.com

PHP:  exit(1);
来源：http://pgk.zdqjudy.top

JS:   process.exit(1)
来源：http://yvn.zhixingplan.top

TS:   process.exit(1)
来源：http://aen.yanxiufei.cn

Java: System.exit(1)
来源：http://qrm.fehbvm.com

Go:   os.Exit(1)
来源：http://tbq.chenjidiqi.icu

Ruby: exit 1
来源：http://ofz.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qqf.wangdashe.top

[M06] 向标准错误输出
来源：http://bxg.xingfuxueyuan.xyz

Py:   print("err", file=sys.stderr)
来源：http://yai.zhoulong.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://bgu.shanyushiyangkeji.top

JS:   console.error("err")
来源：http://gom.xylfe.cn

TS:   console.error("err")
来源：http://wax.vehdjk.com

Java: System.err.println("err")
来源：http://ilz.dashuyun.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://eym.zhixingplan.top

Ruby: warn "err"
来源：http://gkc.snrcjt.cn

C#:   Console.Error.WriteLine("err")
来源：http://btp.iojbl.cn

[M07] 判断是否为主入口
来源：http://yeh.sweek.top

Py:   if __name__ == "__main__":
来源：http://ljd.smart0.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gfv.xylfe.cn

JS:   require.main === module
来源：http://cpl.hywenlv.cn

TS:   require.main === module
来源：http://vxf.gaohongyu789.top

Java: public static void main(String[] args)
来源：http://osb.ppjwa.cn

Go:   func main()
来源：http://wxp.zhiwuduotai.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://hug.chenjidiqi.icu

C#:   static void Main(string[] args)
来源：http://iwn.shanyushiyangkeji.top

[M08] 获取系统与运行时信息
来源：http://gxf.xuanzx.com

Py:   platform.system();  platform.python_version()
来源：http://dmx.redwolf501.top

PHP:  PHP_OS;  phpversion();
来源：http://ysl.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://qyr.jqgufenzy.top

TS:   process.platform;  process.version
来源：http://vgb.316326.xyz

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://cjz.fzhhl.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://rav.cdnleiting.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://yco.hesvh.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://obr.fzhhl.top

================================================================================
来源：http://liu.shuidangran.top

N. 数据结构与算法
来源：http://ars.xinyue.icu

================================================================================
来源：http://njl.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://uwv.quarkkingdee.top

Py:   bisect.bisect_left(arr, x)
来源：http://mul.iojbl.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fze.dianchejie.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://taj.zycfv.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://axx.snrcjt.cn

Java: Arrays.binarySearch(arr, x)
来源：http://mlh.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://won.hongshengwenyu.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://hqx.52xcode.cn

C#:   Array.BinarySearch(arr, x)
来源：http://cet.pycfn.com

[N02] 排序（工程实践用内置实现）
来源：http://ndh.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://iao.vqdsnc.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oad.kuanghao11.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hnn.shanyushiyangkeji.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://dcc.ivvv.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://wao.wangdashe.top

Go:   slices.Sort(arr)
来源：http://tdh.zhixingplan.top

Ruby: arr.sort
来源：http://kmu.xuanzx.com

C#:   Array.Sort(arr);  list.Sort()
来源：http://iis.ybcxt.top

[N03] 快速排序（分治示例）
来源：http://gfk.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://swm.zhaomingkeji.xyz

PHP:  // 递归实现，或用 usort
来源：http://qyd.c1oappe.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mlv.0kj1m.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ehi.xylfe.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://swa.jqgufenzy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bpc.shanyushiyangkeji.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ozi.jyoumei.cn

C#:   // 手写递归，或 Array.Sort
来源：http://qdp.xuanzx.com

[N04] 斐波那契数列
来源：http://ofl.9152youxi.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://xvz.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://arp.chenzaomai.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://hfk.quarkkingdee.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xrs.nanxinkj.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://mbu.shangyingyoupin.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://aeq.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://rex.zhengqikj.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://qwk.nanxinkj.top

[N05] 最大公约数
来源：http://qhu.kuanghao11.cn

Py:   math.gcd(a, b)
来源：http://gqg.pycfn.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://icx.yfazqb.com

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ieu.smart0.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xtg.c1oappe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://rre.nanxinkj.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://lfi.fehbvm.com

Ruby: a.gcd(b)
来源：http://kgu.jyoumei.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lhb.sysykeji.top

[N06] 判断回文字符串
来源：http://kds.gzhubu.top

Py:   s == s[::-1]
来源：http://ldh.shzxlz.cn

PHP:  $s === strrev($s);
来源：http://uzk.ybcxt.top

JS:   s === [...s].reverse().join("")
来源：http://ugv.zhixingplan.top

TS:   s === [...s].reverse().join("")
来源：http://mpi.jinqigufen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://iut.tarul.cn

Go:   // 双指针从两端比较
来源：http://ktq.gotoacloud.top

Ruby: s == s.reverse
来源：http://dji.jinghuilouyu.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cdb.gotoacloud.top

[N07] 两数之和（返回下标）
来源：http://rru.cqqwz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://wur.yongpay.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://mmk.yonumen.top

JS:   // 手写 Map：map.set(v, i)
来源：http://xrl.xylfe.cn

TS:   // 手写 Map<string, number>
来源：http://pet.havefunace.top

Java: // 手写 HashMap
来源：http://buj.316326.xyz


<!-- 参考信息 -->