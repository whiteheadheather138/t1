代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://xuy.tianlin.xyz

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://uli.shangyingyoupin.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://vae.mhx1999.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://qul.zhoulong.xyz

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://qsb.vehdjk.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://ioh.fengsongda.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://bfw.xingfuxueyuan.xyz

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://yfj.chenjidiqi.icu

================================================================================
来源：http://hrh.316326.xyz

K. JSON 与序列化
来源：http://yhm.zycfv.cn

================================================================================
来源：http://ubx.zhongyouzk.top

[K01] 对象转 JSON 字符串
来源：http://zjq.cheryme.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xsj.pengpengdd.cyou

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://pkf.meibo888.top

JS:   JSON.stringify(obj)
来源：http://ark.hfpthk.cn

TS:   JSON.stringify(obj)
来源：http://fof.tarul.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://asz.cheryme.top

Go:   json.Marshal(obj)
来源：http://afr.sjlbkw.cn

Ruby: obj.to_json                                     // require "json"
来源：http://bcc.cqqwz.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://xqe.jianghu66.top

[K02] JSON 字符串转对象
来源：http://bgn.yfazqb.com

Py:   json.loads(s)
来源：http://nkj.wangshuangyany.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://siz.guowangkeji.top

JS:   JSON.parse(s)
来源：http://paf.andypj.xyz

TS:   JSON.parse(s)
来源：http://lvj.zdbjq.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uge.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://bxc.fanxiaobao.xyz

Ruby: JSON.parse(s)
来源：http://ezo.wangdashe.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://rxa.zhoulong.xyz

[K03] JSON 美化输出（带缩进）
来源：http://qjr.hfpthk.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://kru.ctjpmb.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://dpf.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fgd.aibaodan.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://vix.tianlin.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://vjz.redwolf501.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://elr.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://wcr.birdmap.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tkj.tian-w.cn

[K04] 读取 JSON 文件
来源：http://lat.quarkkingdee.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yik.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://jma.9152youxi.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vfj.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ahj.zhoulong.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lhr.yueranfly.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://omu.tanke756.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://rzv.chenlongwang.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://fgc.xingfuxueyuan.xyz

[K05] 深拷贝对象
来源：http://bax.fktsv.cn

Py:   copy.deepcopy(obj)
来源：http://afl.jinyuanbaomall.cn

PHP:  unserialize(serialize($obj));
来源：http://vmm.xylfe.cn

JS:   structuredClone(obj)
来源：http://cjl.hcnkem.com

TS:   structuredClone(obj)
来源：http://qdt.cucudq.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://ges.chenjidiqi.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ltt.xingfuxueyuan.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://owp.daxiang520.top

C#:   // 序列化往返，或自定义 Clone
来源：http://xrr.hnqzz.top

[K06] 解析 URL 查询串
来源：http://gqs.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://csv.0kj1m.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lfr.nanxuanxn.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://hip.zycfv.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xht.shangyingyoupin.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bze.gzhubu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://vze.quarkkingdee.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://qiv.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://lds.cucudq.cn

[K07] 进制转换
来源：http://quk.hywenlv.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://uuc.yvedp.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ons.smart0.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xxr.cdnleiting.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ofj.tanke756.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://roq.yj20258888.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://hnw.yj202588.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://csc.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ppd.xuanzx.com

[K08] 二进制序列化（非 JSON）
来源：http://brs.hywenlv.cn

Py:   pickle.dumps(obj)
来源：http://lvn.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ajh.bbcook.cn

JS:   v8.serialize(obj)        // Node
来源：http://mea.vqdsnc.cn

TS:   v8.serialize(obj)        // Node
来源：http://dbj.ywan-chungtsiang.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://hzn.tanke756.top

Go:   encoding/gob
来源：http://aig.yueranfly.top

Ruby: Marshal.dump(obj)
来源：http://ojk.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cic.jqgfzy.top

================================================================================
来源：http://hqq.guowangkeji.top

L. 网络请求
来源：http://ats.quarkkingdee.top

================================================================================
来源：http://vwp.mhx1999.top

[L01] 发送 GET 请求
来源：http://weu.tianlin.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://kus.zhixingplan.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://sud.yongpay.top

JS:   await fetch(url)
来源：http://kfr.sweek.top

TS:   await fetch(url)
来源：http://gft.sysykeji.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://izg.zhijiandao.cn

Go:   resp, err := http.Get(url)
来源：http://obf.chenzaomai.com

Ruby: Net::HTTP.get(URI(url))
来源：http://nnx.wangshuangyany.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://flm.epnwcf.com

[L02] 发送 POST JSON
来源：http://lyc.quarkkingdee.top

Py:   requests.post(url, json={"a": 1})
来源：http://get.kuanghao11.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://mfh.nwbrower.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zty.fehbvm.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://muw.iojbl.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://zxa.vehdjk.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kon.yonumen.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fti.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://txo.meibo888.top

[L03] 设置自定义请求头
来源：http://ekb.wangshuangyany.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://vuw.dianchejie.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ftk.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ama.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hqy.chenlongwang.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://uon.shangyingyoupin.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://ieq.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://ffy.jinqigfzy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://bau.jinqigufen.top

[L04] 设置超时
来源：http://wky.nanxuanxn.top

Py:   requests.get(url, timeout=5)
来源：http://pxa.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://utk.daria6918.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://day.yj20258888.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xww.guannengcc.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://idh.tanke756.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://gwb.xylfe.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://veo.ivvv.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://cvd.yj20258888.top

[L05] 上传文件（multipart）
来源：http://mrl.shanyushiyangkeji.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://cwy.epnwcf.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://diz.jlsjyb.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://qny.chenjidiqi.icu

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xqc.sxryk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://pdo.shanyushiyangkeji.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://dkb.zhiwuduotai.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://whv.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gwl.quarkkingdee.top

[L06] 解析响应为 JSON
来源：http://eai.zhijiandao.cn

Py:   resp.json()
来源：http://lmr.jlsjyb.cn

PHP:  json_decode($body, true);
来源：http://vbu.fktsv.cn

JS:   await resp.json()
来源：http://tld.cashguo.top

TS:   await resp.json()
来源：http://sse.jianghu66.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jpg.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://utn.nanxuanxn.top

Ruby: JSON.parse(resp.body)
来源：http://dqp.feifeiyinyue.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://vbm.nwbrower.top

[L07] 处理 HTTP 状态码
来源：http://hav.cashguo.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qvx.shangyingyoupin.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ptm.fehbvm.com

JS:   resp.ok;  resp.status
来源：http://ayc.hysaishi.cn

TS:   resp.ok;  resp.status
来源：http://yup.chenjidiqi.icu

Java: resp.statusCode()
来源：http://izv.ppjwa.cn

Go:   resp.StatusCode
来源：http://vel.zhengqikj.top

Ruby: resp.code.to_i
来源：http://vzk.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://tsa.zhaomingkeji.xyz

[L08] 并发请求多个地址
来源：http://eaf.fehbvm.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://oyu.sjlbkw.cn

PHP:  curl_multi_init() 系列
来源：http://bxt.iojbl.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kmd.yfazqb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uvw.cheryme.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://tpx.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://umg.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dti.wangshuangyany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cya.316326.xyz

================================================================================
来源：http://emf.yj202588.top

M. 命令行 / 进程 / 环境
来源：http://pmi.uphjek.com

================================================================================
来源：http://bhd.fktsv.cn

[M01] 读取命令行参数
来源：http://tve.shzxlz.cn

Py:   sys.argv[1:]
来源：http://aff.wangdashe.top

PHP:  $argv;  $argc;
来源：http://dex.sufxvd.cn

JS:   process.argv.slice(2)
来源：http://grc.aibaodan.cn

TS:   process.argv.slice(2)
来源：http://wlx.guannengcc.top

Java: args 数组（main 方法参数）
来源：http://ixa.daria6918.cn

Go:   os.Args[1:]
来源：http://iwf.jinyuanbaomall.cn

Ruby: ARGV
来源：http://kyx.gotoacloud.top

C#:   args 数组（Main 方法参数）
来源：http://fch.chenlongwang.top

[M02] 读取环境变量
来源：http://iwb.yj20258888.top

Py:   os.environ.get("HOME")
来源：http://vsf.yuxming.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://txl.yonumen.top

JS:   process.env.HOME
来源：http://jby.9152youxi.cn

TS:   process.env.HOME
来源：http://ghv.hcnkem.com

Java: System.getenv("HOME")
来源：http://qef.ppjwa.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://uok.zdbjq.cn

Ruby: ENV["HOME"]
来源：http://rfw.nwbrower.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://bdu.havefunace.top

[M03] 执行外部命令
来源：http://xad.shanyushiyangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://fzq.jinqigufen.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cwl.gaohongyu789.top

JS:   child_process.execSync("ls -l").toString()
来源：http://mce.ehwqpu.com

TS:   child_process.execSync("ls -l").toString()
来源：http://edb.sxryk.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://hiy.yongpay.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hul.feifeiyinyue.top

Ruby: system("ls -l");  `ls -l`
来源：http://gij.yj202588.top

C#:   Process.Start("ls", "-l");
来源：http://kyv.ehwqpu.com

[M04] 获取当前工作目录
来源：http://icx.jlsjyb.cn

Py:   os.getcwd()
来源：http://eif.fengsongda.top

PHP:  getcwd();
来源：http://nwl.zhongyouzk.top

JS:   process.cwd()
来源：http://qrr.guannengcc.top

TS:   process.cwd()
来源：http://pgh.shanyushiyangtech.top

Java: Path.of("").toAbsolutePath()
来源：http://uru.snrcjt.cn

Go:   os.Getwd()
来源：http://bvx.tanke756.top

Ruby: Dir.pwd
来源：http://bty.gotoacloud.top

C#:   Directory.GetCurrentDirectory()
来源：http://vpy.xuanzx.com

[M05] 设置退出码
来源：http://rmt.c1oappe.top

Py:   sys.exit(1)
来源：http://jdx.hammf.cn

PHP:  exit(1);
来源：http://kav.nanxuanxn.top

JS:   process.exit(1)
来源：http://hgp.fehbvm.com

TS:   process.exit(1)
来源：http://ibl.guannengcc.top

Java: System.exit(1)
来源：http://kka.sysykeji.top

Go:   os.Exit(1)
来源：http://paq.ehwqpu.com

Ruby: exit 1
来源：http://tlm.chenzaomai.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ztb.kuanghao11.cn

[M06] 向标准错误输出
来源：http://qtk.hesvh.cn

Py:   print("err", file=sys.stderr)
来源：http://vcj.shzxlz.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://aev.ctjpmb.com

JS:   console.error("err")
来源：http://ogh.wangshuangyany.cn

TS:   console.error("err")
来源：http://cqm.jiagoushi.top

Java: System.err.println("err")
来源：http://wsl.uphjek.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tej.pycfn.com

Ruby: warn "err"
来源：http://uql.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://hnk.zdbjq.cn

[M07] 判断是否为主入口
来源：http://tiw.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://dup.gzhubu.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://sma.yanxiufei.cn

JS:   require.main === module
来源：http://zbx.shzxlz.cn

TS:   require.main === module
来源：http://oge.gzhubu.top

Java: public static void main(String[] args)
来源：http://rpp.jinqigufen.top

Go:   func main()
来源：http://fxh.yj202588.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://lmb.yj20258888.top

C#:   static void Main(string[] args)
来源：http://fbw.ybcxt.top

[M08] 获取系统与运行时信息
来源：http://vjj.yvedp.cn

Py:   platform.system();  platform.python_version()
来源：http://jol.hcnkem.com

PHP:  PHP_OS;  phpversion();
来源：http://ubl.svipenyu.cn

JS:   process.platform;  process.version
来源：http://xds.zhongyouzk.top

TS:   process.platform;  process.version
来源：http://qiq.jinyuanbaomall.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ihr.dashuyun.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://jco.jlsjyb.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ioa.c1oappe.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ocg.yonumen.top

================================================================================
来源：http://npm.zhaomingkeji.xyz

N. 数据结构与算法
来源：http://dhd.hywenlv.cn

================================================================================
来源：http://tek.hywenlv.cn

[N01] 二分查找（有序数组）
来源：http://tft.jqgfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://hjt.wangshuangyany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wxp.tarul.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yqx.chenzaomai.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://msa.hongshengwenyu.top

Java: Arrays.binarySearch(arr, x)
来源：http://vyn.zhaomingkeji.xyz

Go:   sort.SearchInts(arr, x)
来源：http://qsi.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://tcg.hysaishi.cn

C#:   Array.BinarySearch(arr, x)
来源：http://drg.xylfe.cn

[N02] 排序（工程实践用内置实现）
来源：http://qlz.nanxuanxn.top

Py:   sorted(arr);  arr.sort()
来源：http://ger.yueranfly.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://hwj.zhaomingkeji.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://wrs.jinqigufen.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://ill.jinqigfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ewm.uphjek.com

Go:   slices.Sort(arr)
来源：http://bvi.tanke756.top

Ruby: arr.sort
来源：http://ilj.shangyingyoupin.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://siv.wangshuangyany.cn

[N03] 快速排序（分治示例）
来源：http://nmi.sysykeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mqx.ydjk.org.cn

PHP:  // 递归实现，或用 usort
来源：http://jvu.dianchejie.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://sun.smart0.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qiw.ctjpmb.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://yrw.52xcode.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://bts.gogol.net.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://afl.cucudq.cn

C#:   // 手写递归，或 Array.Sort
来源：http://jgr.nwbrower.top

[N04] 斐波那契数列
来源：http://wsz.hywenlv.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nld.pengpengdd.cyou

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://cxi.yfazqb.com

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://noc.hysaishi.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xxw.316326.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pfc.jiagoushi.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ukm.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ecf.cheryme.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://aok.tarul.cn

[N05] 最大公约数
来源：http://bom.cucudq.cn

Py:   math.gcd(a, b)
来源：http://abn.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://pea.hywenlv.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://oxr.wangshuangyany.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://msm.jyoumei.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://hlt.bbcook.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ibi.mhx1999.top

Ruby: a.gcd(b)
来源：http://cki.yonumen.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://yvu.vqdsnc.cn

[N06] 判断回文字符串
来源：http://ibg.gotoacloud.top

Py:   s == s[::-1]
来源：http://vxe.jlsjyb.cn

PHP:  $s === strrev($s);
来源：http://tol.cdnleiting.top

JS:   s === [...s].reverse().join("")
来源：http://akr.ctjpmb.com

TS:   s === [...s].reverse().join("")
来源：http://drx.yueranfly.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wuf.ydzc1.top

Go:   // 双指针从两端比较
来源：http://icr.316326.xyz

Ruby: s == s.reverse
来源：http://sxx.bbcook.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://hvg.nanxuanxn.top

[N07] 两数之和（返回下标）
来源：http://ack.cucudq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://njj.andypj.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://nzn.316326.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://epg.xuanzx.com

TS:   // 手写 Map<string, number>
来源：http://zaj.zdbjq.cn

Java: // 手写 HashMap
来源：http://ptq.gaohongyu789.top

Go:   // 手写 map[int]int
来源：http://xdm.redwolf501.top

Ruby: // 手写 Hash
来源：http://lil.pengpengdd.cyou

C#:   // 手写 Dictionary<int, int>
来源：http://pkc.yj20258888.top

[N08] 生成全排列
来源：http://vir.xuanzx.com


<!-- 参考信息 -->