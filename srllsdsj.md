代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://sua.jlsjyb.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://sxb.shuidangran.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://doa.fktsv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://bbz.haohaochexian.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://zaj.sxryk.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kes.tanke756.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://maj.shuidangran.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://woo.gotoacloud.top

================================================================================
来源：http://ksi.gogol.net.cn

K. JSON 与序列化
来源：http://dwp.shanyushiyangtech.top

================================================================================
来源：http://tpe.xylfe.cn

[K01] 对象转 JSON 字符串
来源：http://nzp.tarul.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jhd.nanxuanxn.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://utr.sjlbkw.cn

JS:   JSON.stringify(obj)
来源：http://ejk.sweek.top

TS:   JSON.stringify(obj)
来源：http://gor.zhoulong.xyz

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://shv.c1oappe.top

Go:   json.Marshal(obj)
来源：http://vkg.havefunace.top

Ruby: obj.to_json                                     // require "json"
来源：http://nsa.snrcjt.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://rzj.tarul.cn

[K02] JSON 字符串转对象
来源：http://wlk.hywenlv.cn

Py:   json.loads(s)
来源：http://ojs.birdmap.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://qjb.hcnkem.com

JS:   JSON.parse(s)
来源：http://sdf.zhijiandao.cn

TS:   JSON.parse(s)
来源：http://oye.jianghu66.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://vjn.hnxiangtu.top

Go:   json.Unmarshal(data, &v)
来源：http://klh.jqgfzy.top

Ruby: JSON.parse(s)
来源：http://qlt.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://jyi.ydjk.org.cn

[K03] JSON 美化输出（带缩进）
来源：http://gvm.zhengqikj.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://oyi.hywenlv.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://rfu.guannengcc.top

JS:   JSON.stringify(obj, null, 2)
来源：http://fve.jlsjyb.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://ija.jqgfzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://iww.gaohongyu789.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://coy.daria6918.cn

Ruby: JSON.pretty_generate(obj)
来源：http://rvr.daxiang520.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kpb.pycfn.com

[K04] 读取 JSON 文件
来源：http://bcc.mhx1999.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://vfn.yanxiufei.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zxz.yangfankeji.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fre.aibaodan.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://txh.jqgufenzy.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://lov.hysaishi.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://hgi.hongshengwenyu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://bnl.jianghu66.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ruw.jinghuilouyu.cn

[K05] 深拷贝对象
来源：http://rny.hysaishi.cn

Py:   copy.deepcopy(obj)
来源：http://peu.hywenlv.cn

PHP:  unserialize(serialize($obj));
来源：http://lur.vqdsnc.cn

JS:   structuredClone(obj)
来源：http://fno.jianghu66.top

TS:   structuredClone(obj)
来源：http://zyz.ehwqpu.com

Java: // 手写拷贝构造，或序列化往返
来源：http://jqu.gaohongyu789.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ijg.zhoulong.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://kuo.hesvh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vqm.wangshuangyany.cn

[K06] 解析 URL 查询串
来源：http://qgi.pycfn.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://acc.sufxvd.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://hun.hnxiangtu.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://fjo.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://kjw.nanxuanxn.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bep.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://uef.kuanghao11.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://cmk.ywan-chungtsiang.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://gvi.cashguo.top

[K07] 进制转换
来源：http://iis.mhx1999.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://otc.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://wzp.iojbl.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://zdi.xylfe.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://icg.ivvv.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://fjj.c1oappe.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://wki.bbcook.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ntf.xingfuxueyuan.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://yoj.zhaomingkeji.xyz

[K08] 二进制序列化（非 JSON）
来源：http://dkr.chenjidiqi.icu

Py:   pickle.dumps(obj)
来源：http://ikr.cucudq.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://ktf.jinqigufen.top

JS:   v8.serialize(obj)        // Node
来源：http://izr.snrcjt.cn

TS:   v8.serialize(obj)        // Node
来源：http://xnr.haohaochexian.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://log.havefunace.top

Go:   encoding/gob
来源：http://dsh.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://oyo.uphjek.com

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://fpn.yj20258.top

================================================================================
来源：http://btr.xinyue.icu

L. 网络请求
来源：http://drf.yueranfly.top

================================================================================
来源：http://stq.ppjwa.cn

[L01] 发送 GET 请求
来源：http://cjh.cdnleiting.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://sbe.hnqzz.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://rga.yangfankeji.com

JS:   await fetch(url)
来源：http://ldl.hammf.cn

TS:   await fetch(url)
来源：http://vos.zhijiandao.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://kzu.yj20258.top

Go:   resp, err := http.Get(url)
来源：http://esz.xuanzx.com

Ruby: Net::HTTP.get(URI(url))
来源：http://mlx.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://amb.chenzaomai.com

[L02] 发送 POST JSON
来源：http://zcq.zhoulong.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://csk.dashuyun.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://laq.jinghuilouyu.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://tvv.sysykeji.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://juu.hfpthk.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://vei.52xcode.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://mec.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://uei.zhengqikj.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ukk.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://gab.9152youxi.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ofr.zhengqikj.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://myv.hesvh.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zat.chenlongwang.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://jfw.shanyushiyangtech.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://rto.chenjidiqi.icu

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jsj.yj20258.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cby.jinghuilouyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://anu.daria6918.cn

[L04] 设置超时
来源：http://hzv.sufxvd.cn

Py:   requests.get(url, timeout=5)
来源：http://vfe.cashguo.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://glk.jlsjyb.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://wct.fehbvm.com

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cmu.nanxuanxn.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wbr.yuanzhike.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://shp.nwbrower.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://sps.daxiang520.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://xqc.chenjidiqi.icu

[L05] 上传文件（multipart）
来源：http://kxz.jyoumei.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nhn.hywenlv.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://gzp.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://itp.tanke756.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://fer.yonumen.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://evh.vehdjk.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ygv.meibo888.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://fjn.vehdjk.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://blg.yuanzhike.top

[L06] 解析响应为 JSON
来源：http://auv.jlsjyb.cn

Py:   resp.json()
来源：http://smb.iojbl.cn

PHP:  json_decode($body, true);
来源：http://hjs.zdqjudy.top

JS:   await resp.json()
来源：http://axq.jinqigufen.top

TS:   await resp.json()
来源：http://hiz.316326.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ehq.9152youxi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://pzm.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://lwy.zhaomingkeji.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xma.hywenlv.cn

[L07] 处理 HTTP 状态码
来源：http://alc.hfpthk.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vus.zhixingplan.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://xdb.meibo888.top

JS:   resp.ok;  resp.status
来源：http://kbe.fengsongda.top

TS:   resp.ok;  resp.status
来源：http://dkl.0kj1m.cn

Java: resp.statusCode()
来源：http://ogp.zhengqikj.top

Go:   resp.StatusCode
来源：http://jsg.gogol.net.cn

Ruby: resp.code.to_i
来源：http://yzy.svipenyu.cn

C#:   (int)resp.StatusCode
来源：http://uhx.yueranfly.top

[L08] 并发请求多个地址
来源：http://xxx.andypj.xyz

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://dyf.yangfankeji.com

PHP:  curl_multi_init() 系列
来源：http://vsl.shanyushiyangtech.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bxm.gotoacloud.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://obf.pycfn.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ghq.wangshuangyany.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://okb.bbcook.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://xlr.hywenlv.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://mif.wangdashe.top

================================================================================
来源：http://cwk.pycfn.com

M. 命令行 / 进程 / 环境
来源：http://fwi.shuidangran.top

================================================================================
来源：http://rnv.meibo888.top

[M01] 读取命令行参数
来源：http://xsb.ydjk.org.cn

Py:   sys.argv[1:]
来源：http://qaq.pengpengdd.cyou

PHP:  $argv;  $argc;
来源：http://cxj.9152youxi.cn

JS:   process.argv.slice(2)
来源：http://ukm.cashguo.top

TS:   process.argv.slice(2)
来源：http://ben.chenzaomai.com

Java: args 数组（main 方法参数）
来源：http://aes.daxiang520.top

Go:   os.Args[1:]
来源：http://tzj.zycfv.cn

Ruby: ARGV
来源：http://uhj.haohaochexian.top

C#:   args 数组（Main 方法参数）
来源：http://lra.fehbvm.com

[M02] 读取环境变量
来源：http://ool.jinqigfzy.top

Py:   os.environ.get("HOME")
来源：http://nbb.gogol.net.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://bmq.tian-w.cn

JS:   process.env.HOME
来源：http://lmu.gotoacloud.top

TS:   process.env.HOME
来源：http://ibk.aibaodan.cn

Java: System.getenv("HOME")
来源：http://niu.ehwqpu.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nhz.pycfn.com

Ruby: ENV["HOME"]
来源：http://lvp.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://lnx.shzxlz.cn

[M03] 执行外部命令
来源：http://oew.ybcxt.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://idk.fzhhl.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://osp.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://che.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://hjc.yangfankeji.com

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sem.hnxiangtu.top

Go:   exec.Command("ls", "-l").Output()
来源：http://srv.jinghuilouyu.cn

Ruby: system("ls -l");  `ls -l`
来源：http://acv.guowangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://rrj.xylfe.cn

[M04] 获取当前工作目录
来源：http://izj.kuanghao11.cn

Py:   os.getcwd()
来源：http://afm.quarkkingdee.top

PHP:  getcwd();
来源：http://grt.ydzc1.top

JS:   process.cwd()
来源：http://wir.cqqwz.cn

TS:   process.cwd()
来源：http://avq.hongshengwenyu.top

Java: Path.of("").toAbsolutePath()
来源：http://nrp.sweek.top

Go:   os.Getwd()
来源：http://pwp.fzhhl.top

Ruby: Dir.pwd
来源：http://pht.vqdsnc.cn

C#:   Directory.GetCurrentDirectory()
来源：http://qdu.guowangkeji.top

[M05] 设置退出码
来源：http://tsk.zhoulong.xyz

Py:   sys.exit(1)
来源：http://itn.fzhhl.top

PHP:  exit(1);
来源：http://uho.0kj1m.cn

JS:   process.exit(1)
来源：http://bcv.yuxming.cn

TS:   process.exit(1)
来源：http://uby.smart0.xyz

Java: System.exit(1)
来源：http://opu.sxryk.cn

Go:   os.Exit(1)
来源：http://lst.zhiwuduotai.top

Ruby: exit 1
来源：http://hsq.yangfankeji.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qft.tian-w.cn

[M06] 向标准错误输出
来源：http://qag.shanyushiyangtech.top

Py:   print("err", file=sys.stderr)
来源：http://fcq.andypj.xyz

PHP:  fwrite(STDERR, "err\n");
来源：http://aau.quarkkingdee.top

JS:   console.error("err")
来源：http://hha.xylfe.cn

TS:   console.error("err")
来源：http://wbe.shanyushiyangkeji.top

Java: System.err.println("err")
来源：http://zxs.redwolf501.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://yth.fengsongda.top

Ruby: warn "err"
来源：http://yjj.fzhhl.top

C#:   Console.Error.WriteLine("err")
来源：http://gkh.sysykeji.top

[M07] 判断是否为主入口
来源：http://cus.hesvh.cn

Py:   if __name__ == "__main__":
来源：http://spl.aibaodan.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://ucx.gzhubu.top

JS:   require.main === module
来源：http://dsc.c1oappe.top

TS:   require.main === module
来源：http://zzx.yuanzhike.top

Java: public static void main(String[] args)
来源：http://cky.redwolf501.top

Go:   func main()
来源：http://mfn.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://tex.hcnkem.com

C#:   static void Main(string[] args)
来源：http://afc.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://jqp.cheryme.top

Py:   platform.system();  platform.python_version()
来源：http://cbj.ydzc1.top

PHP:  PHP_OS;  phpversion();
来源：http://bmj.fktsv.cn

JS:   process.platform;  process.version
来源：http://dzz.vqdsnc.cn

TS:   process.platform;  process.version
来源：http://yuw.fehbvm.com

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rts.shuidangran.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ckq.xuetiantiany.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://omv.xziqi.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://mqq.redwolf501.top

================================================================================
来源：http://das.pengpengdd.cyou

N. 数据结构与算法
来源：http://dvk.aizwys.cn

================================================================================
来源：http://yfd.yvedp.cn

[N01] 二分查找（有序数组）
来源：http://raz.0kj1m.cn

Py:   bisect.bisect_left(arr, x)
来源：http://sdl.xuetiantiany.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://rif.zdbjq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://vrm.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ybq.yfazqb.com

Java: Arrays.binarySearch(arr, x)
来源：http://tlo.xylfe.cn

Go:   sort.SearchInts(arr, x)
来源：http://yxo.sjlbkw.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://jrv.zhengqikj.top

C#:   Array.BinarySearch(arr, x)
来源：http://jvu.guowangkeji.top

[N02] 排序（工程实践用内置实现）
来源：http://ing.aizwys.cn

Py:   sorted(arr);  arr.sort()
来源：http://rny.jqgufenzy.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://afk.jianghu66.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sis.kuanghao11.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://hdx.jqgfzy.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://zeg.9152youxi.cn

Go:   slices.Sort(arr)
来源：http://qdz.gaohongyu789.top

Ruby: arr.sort
来源：http://wjk.sysykeji.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://yqx.jyoumei.cn

[N03] 快速排序（分治示例）
来源：http://szo.yanxiufei.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://qja.quarkkingdee.top

PHP:  // 递归实现，或用 usort
来源：http://tlv.redwolf501.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vov.shzxlz.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zri.zhaomingkeji.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://xax.zdqjudy.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ows.cashguo.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://zvd.andypj.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://txh.yuxming.cn

[N04] 斐波那契数列
来源：http://ulm.aizwys.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://nsv.shanyushiyangkeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://avr.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qpq.ydzc1.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ser.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://pow.zdqjudy.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://efv.yvedp.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ene.havefunace.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ddb.daria6918.cn

[N05] 最大公约数
来源：http://tjs.iojbl.cn

Py:   math.gcd(a, b)
来源：http://ooy.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://iql.gaohongyu789.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tiq.ybcxt.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hyp.9152youxi.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qkj.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wdp.ywan-chungtsiang.top

Ruby: a.gcd(b)
来源：http://idg.zhaomingkeji.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pkt.jianghu66.top

[N06] 判断回文字符串
来源：http://mkj.xylfe.cn

Py:   s == s[::-1]
来源：http://aks.yj202588.top

PHP:  $s === strrev($s);
来源：http://teo.zhixingplan.top

JS:   s === [...s].reverse().join("")
来源：http://nsr.xingfuxueyuan.xyz

TS:   s === [...s].reverse().join("")
来源：http://bet.ydjk.org.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://wqc.yfazqb.com

Go:   // 双指针从两端比较
来源：http://ojg.zhaomingkeji.xyz

Ruby: s == s.reverse
来源：http://aqy.fehbvm.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://dfz.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://avm.tianlin.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bwk.zhiwuduotai.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://woa.hnqzz.top

JS:   // 手写 Map：map.set(v, i)
来源：http://ake.chenjidiqi.icu

TS:   // 手写 Map<string, number>
来源：http://pab.ivvv.top

Java: // 手写 HashMap
来源：http://nip.tarul.cn

Go:   // 手写 map[int]int
来源：http://bhh.yj20258.top

Ruby: // 手写 Hash
来源：http://tei.yueranfly.top

C#:   // 手写 Dictionary<int, int>
来源：http://voo.zhaomingkeji.xyz

[N08] 生成全排列
来源：http://mwz.yuxming.cn


<!-- 参考信息 -->