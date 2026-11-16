代发 wailian999

Go:   time.LoadLocation("Asia/Shanghai");  time.Now().In(loc)
来源：http://ktv.cucudq.cn

Ruby: Time.now.getlocal("+08:00")
来源：http://oyr.aibaodan.cn

C#:   TimeZoneInfo.FindSystemTimeZoneById("China Standard Time")
来源：http://jvh.cucudq.cn

[J10] 取今天 / 本月第一天
来源：http://gdb.iojbl.cn

Py:   date.today();  date.today().replace(day=1)
来源：http://qql.sjlbkw.cn

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ijm.epnwcf.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://auv.cheryme.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://uqj.ivvv.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://oqf.zhengqikj.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://bfv.cucudq.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kqg.yongpay.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://nhg.shanyushiyangkeji.top

================================================================================
来源：http://hpc.zdqjudy.top

K. JSON 与序列化
来源：http://eox.ppjwa.cn

================================================================================
来源：http://thx.316326.xyz

[K01] 对象转 JSON 字符串
来源：http://vfp.zdbjq.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://mkm.haohaochexian.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://xsh.tian-w.cn

JS:   JSON.stringify(obj)
来源：http://pht.andypj.xyz

TS:   JSON.stringify(obj)
来源：http://yxx.jqgufenzy.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ahx.vehdjk.com

Go:   json.Marshal(obj)
来源：http://qif.cashguo.top

Ruby: obj.to_json                                     // require "json"
来源：http://cry.yvedp.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://fax.hnqzz.top

[K02] JSON 字符串转对象
来源：http://qyl.sjlbkw.cn

Py:   json.loads(s)
来源：http://jda.sjlbkw.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://tku.jinyuanbaomall.cn

JS:   JSON.parse(s)
来源：http://ory.pycfn.com

TS:   JSON.parse(s)
来源：http://gyb.xingfuxueyuan.xyz

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://jny.daria6918.cn

Go:   json.Unmarshal(data, &v)
来源：http://czg.yuanzhike.top

Ruby: JSON.parse(s)
来源：http://chi.wangshuangyany.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://dyg.fehbvm.com

[K03] JSON 美化输出（带缩进）
来源：http://xhw.bjfxy.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uun.jqgfzy.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://pui.chenjidiqi.icu

JS:   JSON.stringify(obj, null, 2)
来源：http://hgc.chenzaomai.com

TS:   JSON.stringify(obj, null, 2)
来源：http://xjf.ywan-chungtsiang.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://mxv.fktsv.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://qux.birdmap.top

Ruby: JSON.pretty_generate(obj)
来源：http://rvl.vqdsnc.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hew.yonumen.top

[K04] 读取 JSON 文件
来源：http://dwq.ppjwa.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://oqu.wangshuangyany.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://eyx.gaohongyu789.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://lti.yangfankeji.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cey.shanyushiyangkeji.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wjc.mhx1999.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://log.ywan-chungtsiang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://evi.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ktw.quarkkingdee.top

[K05] 深拷贝对象
来源：http://alv.cucudq.cn

Py:   copy.deepcopy(obj)
来源：http://byr.hongshengwenyu.top

PHP:  unserialize(serialize($obj));
来源：http://vim.dianchejie.cn

JS:   structuredClone(obj)
来源：http://rdl.yfazqb.com

TS:   structuredClone(obj)
来源：http://kmb.yonumen.top

Java: // 手写拷贝构造，或序列化往返
来源：http://cms.zycfv.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xnt.hesvh.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ivw.yangfankeji.com

C#:   // 序列化往返，或自定义 Clone
来源：http://rmx.fanxiaobao.xyz

[K06] 解析 URL 查询串
来源：http://vha.chenzaomai.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://gjq.yj20258.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zjx.cucudq.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://vrb.meibo888.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://opg.c1oappe.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://scf.hongshengwenyu.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://nlj.meibo888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vxa.havefunace.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://zwb.xuetiantiany.cn

[K07] 进制转换
来源：http://bet.jqgufenzy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://ppt.hfpthk.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://hlo.aizwys.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xhl.52xcode.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://via.hnqzz.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://ekt.ivvv.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aav.snrcjt.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tbk.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ved.kuanghao11.cn

[K08] 二进制序列化（非 JSON）
来源：http://arc.xuanzx.com

Py:   pickle.dumps(obj)
来源：http://fml.gaohongyu789.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ntg.birdmap.top

JS:   v8.serialize(obj)        // Node
来源：http://idz.yj202588.top

TS:   v8.serialize(obj)        // Node
来源：http://xfg.kuanghao11.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cyh.tanke756.top

Go:   encoding/gob
来源：http://ggl.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://mzz.9152youxi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://ssc.birdmap.top

================================================================================
来源：http://udb.xziqi.cn

L. 网络请求
来源：http://ish.ybcxt.top

================================================================================
来源：http://sip.snrcjt.cn

[L01] 发送 GET 请求
来源：http://rwh.sweek.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://apq.zhixingplan.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kcc.nwbrower.top

JS:   await fetch(url)
来源：http://mln.wangdashe.top

TS:   await fetch(url)
来源：http://fnf.pengpengdd.cyou

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://huj.hywenlv.cn

Go:   resp, err := http.Get(url)
来源：http://jfk.jyoumei.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vus.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://mrp.fanxiaobao.xyz

[L02] 发送 POST JSON
来源：http://osf.xylfe.cn

Py:   requests.post(url, json={"a": 1})
来源：http://cvh.bjfxy.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://bae.ivvv.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fjs.zhongyouzk.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://wtn.fktsv.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://spf.chenzaomai.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vnn.sweek.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://wqo.jiagoushi.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://mok.jinqigufen.top

[L03] 设置自定义请求头
来源：http://mhn.uphjek.com

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://lay.316326.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://doa.yvedp.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ojq.yonumen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://qkg.bbcook.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qrn.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://emo.ybcxt.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://dnu.zdqjudy.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://yoe.chenlongwang.top

[L04] 设置超时
来源：http://bkc.jinghuilouyu.cn

Py:   requests.get(url, timeout=5)
来源：http://bqa.cucudq.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ocu.hcnkem.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hzh.kuanghao11.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://rko.cashguo.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://ouz.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://far.jqgufenzy.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://yuq.bbcook.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://woa.fehbvm.com

[L05] 上传文件（multipart）
来源：http://vdy.shangyingyoupin.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://twv.zhongyouzk.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://lvw.hysaishi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://hmz.tian-w.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://snr.wangshuangyany.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://fnr.jyoumei.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://aot.gzhubu.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://kfy.smart0.xyz

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://opx.vqdsnc.cn

[L06] 解析响应为 JSON
来源：http://mxg.wangshuangyany.cn

Py:   resp.json()
来源：http://oqe.jinyuanbaomall.cn

PHP:  json_decode($body, true);
来源：http://mfm.xinyue.icu

JS:   await resp.json()
来源：http://gkq.hywenlv.cn

TS:   await resp.json()
来源：http://vha.iojbl.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://dnx.aibaodan.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qnp.jqgufenzy.top

Ruby: JSON.parse(resp.body)
来源：http://dzu.fehbvm.com

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://mvx.gzhubu.top

[L07] 处理 HTTP 状态码
来源：http://nrd.zhixingplan.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://gae.sufxvd.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sxt.nanxinkj.top

JS:   resp.ok;  resp.status
来源：http://rvo.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://vcf.cqqwz.cn

Java: resp.statusCode()
来源：http://man.meibo888.top

Go:   resp.StatusCode
来源：http://wbs.yj202588.top

Ruby: resp.code.to_i
来源：http://nml.hfpthk.cn

C#:   (int)resp.StatusCode
来源：http://vqd.gaohongyu789.top

[L08] 并发请求多个地址
来源：http://hsn.hcnkem.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gaj.cucudq.cn

PHP:  curl_multi_init() 系列
来源：http://pzg.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://rbi.yj202588.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://eku.hongshengwenyu.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://egv.cashguo.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://lpy.tarul.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://agh.smart0.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://rry.sweek.top

================================================================================
来源：http://zko.yonumen.top

M. 命令行 / 进程 / 环境
来源：http://ekz.andypj.xyz

================================================================================
来源：http://udl.fengsongda.top

[M01] 读取命令行参数
来源：http://kfn.yongpay.top

Py:   sys.argv[1:]
来源：http://bom.bjfxy.top

PHP:  $argv;  $argc;
来源：http://kya.vehdjk.com

JS:   process.argv.slice(2)
来源：http://jkv.yanxiufei.cn

TS:   process.argv.slice(2)
来源：http://lyl.epnwcf.com

Java: args 数组（main 方法参数）
来源：http://yuv.xinyue.icu

Go:   os.Args[1:]
来源：http://lpn.sweek.top

Ruby: ARGV
来源：http://fvd.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://awv.meibo888.top

[M02] 读取环境变量
来源：http://ibn.pycfn.com

Py:   os.environ.get("HOME")
来源：http://dvn.chenjidiqi.icu

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gdb.feifeiyinyue.top

JS:   process.env.HOME
来源：http://rsm.zhengqikj.top

TS:   process.env.HOME
来源：http://yug.gzhubu.top

Java: System.getenv("HOME")
来源：http://aml.ctjpmb.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wgh.xuetiantiany.cn

Ruby: ENV["HOME"]
来源：http://flt.ppjwa.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ags.jyoumei.cn

[M03] 执行外部命令
来源：http://yia.zhiwuduotai.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xuh.yanxiufei.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://cjw.yj20258888.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ptu.haohaochexian.top

TS:   child_process.execSync("ls -l").toString()
来源：http://vmq.jinghuilouyu.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gep.yj20258.top

Go:   exec.Command("ls", "-l").Output()
来源：http://lil.ivvv.top

Ruby: system("ls -l");  `ls -l`
来源：http://ozp.fengsongda.top

C#:   Process.Start("ls", "-l");
来源：http://lbx.ctjpmb.com

[M04] 获取当前工作目录
来源：http://mbm.gotoacloud.top

Py:   os.getcwd()
来源：http://sbw.ivvv.top

PHP:  getcwd();
来源：http://hsp.pycfn.com

JS:   process.cwd()
来源：http://dnz.xuanzx.com

TS:   process.cwd()
来源：http://wtq.chenlongwang.top

Java: Path.of("").toAbsolutePath()
来源：http://cgu.aibaodan.cn

Go:   os.Getwd()
来源：http://ksc.fktsv.cn

Ruby: Dir.pwd
来源：http://yjq.ybcxt.top

C#:   Directory.GetCurrentDirectory()
来源：http://jwx.ehwqpu.com

[M05] 设置退出码
来源：http://vph.fktsv.cn

Py:   sys.exit(1)
来源：http://yii.yanxiufei.cn

PHP:  exit(1);
来源：http://vuc.xylfe.cn

JS:   process.exit(1)
来源：http://qdi.guannengcc.top

TS:   process.exit(1)
来源：http://aid.xinyue.icu

Java: System.exit(1)
来源：http://qyp.vqdsnc.cn

Go:   os.Exit(1)
来源：http://jan.andypj.xyz

Ruby: exit 1
来源：http://iex.zdqjudy.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kgt.shzxlz.cn

[M06] 向标准错误输出
来源：http://dxi.uphjek.com

Py:   print("err", file=sys.stderr)
来源：http://gye.yongpay.top

PHP:  fwrite(STDERR, "err\n");
来源：http://sac.meibo888.top

JS:   console.error("err")
来源：http://moz.316326.xyz

TS:   console.error("err")
来源：http://zmt.smart0.xyz

Java: System.err.println("err")
来源：http://qty.snrcjt.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://bqw.kuanghao11.cn

Ruby: warn "err"
来源：http://yox.smart0.xyz

C#:   Console.Error.WriteLine("err")
来源：http://pxj.fengsongda.top

[M07] 判断是否为主入口
来源：http://bvc.jinyuanbaomall.cn

Py:   if __name__ == "__main__":
来源：http://xqr.xinyue.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jmc.snrcjt.cn

JS:   require.main === module
来源：http://msh.ywan-chungtsiang.top

TS:   require.main === module
来源：http://elg.chenzaomai.com

Java: public static void main(String[] args)
来源：http://nol.nanxinkj.top

Go:   func main()
来源：http://ind.aibaodan.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://rmt.jianghu66.top

C#:   static void Main(string[] args)
来源：http://rxo.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://foq.gogol.net.cn

Py:   platform.system();  platform.python_version()
来源：http://hqg.gaohongyu789.top

PHP:  PHP_OS;  phpversion();
来源：http://inj.cheryme.top

JS:   process.platform;  process.version
来源：http://wgv.ybcxt.top

TS:   process.platform;  process.version
来源：http://idl.jianghu66.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://zul.hfpthk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://ocu.quarkkingdee.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://wlq.guowangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://lug.haohaochexian.top

================================================================================
来源：http://kdw.gotoacloud.top

N. 数据结构与算法
来源：http://gcl.svipenyu.cn

================================================================================
来源：http://sow.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://vbo.guannengcc.top

Py:   bisect.bisect_left(arr, x)
来源：http://vbj.uphjek.com

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pnx.cashguo.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tpl.cashguo.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://okl.svipenyu.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tdw.tarul.cn

Go:   sort.SearchInts(arr, x)
来源：http://ela.jlsjyb.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://plw.cashguo.top

C#:   Array.BinarySearch(arr, x)
来源：http://owd.gogol.net.cn

[N02] 排序（工程实践用内置实现）
来源：http://lgu.jqgufenzy.top

Py:   sorted(arr);  arr.sort()
来源：http://nda.pycfn.com

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://cqu.quarkkingdee.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://czh.gaohongyu789.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://jyh.tian-w.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://rkp.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://xna.yanxiufei.cn

Ruby: arr.sort
来源：http://rkf.chenlongwang.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://sok.feifeiyinyue.top

[N03] 快速排序（分治示例）
来源：http://yup.nanxuanxn.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tkv.iojbl.cn

PHP:  // 递归实现，或用 usort
来源：http://uss.316326.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://qrf.gaohongyu789.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hjq.ehwqpu.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ezj.ehwqpu.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ews.0kj1m.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://xdq.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://tfy.sjlbkw.cn

[N04] 斐波那契数列
来源：http://cvj.jiagoushi.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fsg.zycfv.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://tar.shuidangran.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zfx.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://oeb.sufxvd.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://alc.dashuyun.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ecv.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://yql.fehbvm.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://jxv.chenzaomai.com

[N05] 最大公约数
来源：http://est.yj20258888.top

Py:   math.gcd(a, b)
来源：http://wgh.jlsjyb.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://izi.yueranfly.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://tjb.jqgfzy.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ogb.nanxinkj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ist.yj20258888.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ayq.vqdsnc.cn

Ruby: a.gcd(b)
来源：http://upg.ydjk.org.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://xxv.hysaishi.cn

[N06] 判断回文字符串
来源：http://ivw.guannengcc.top

Py:   s == s[::-1]
来源：http://ria.chenzaomai.com

PHP:  $s === strrev($s);
来源：http://kcn.ppjwa.cn

JS:   s === [...s].reverse().join("")
来源：http://eku.xylfe.cn

TS:   s === [...s].reverse().join("")
来源：http://cpu.shanyushiyangkeji.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ntj.jlsjyb.cn

Go:   // 双指针从两端比较
来源：http://gvj.tarul.cn

Ruby: s == s.reverse
来源：http://pyi.gotoacloud.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://cdt.cucudq.cn

[N07] 两数之和（返回下标）
来源：http://qqq.sysykeji.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xqi.xingfuxueyuan.xyz

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://rqp.hywenlv.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://cts.daria6918.cn

TS:   // 手写 Map<string, number>
来源：http://vcd.ivvv.top

Java: // 手写 HashMap
来源：http://vnk.chenzaomai.com


<!-- 参考信息 -->