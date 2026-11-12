代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://ypj.zhongyouzk.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://ond.yonumen.top

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://yla.zhiwuduotai.top

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://abu.tanke756.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://cka.ctjpmb.com

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://yhk.hongshengwenyu.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mfe.jqgfzy.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://qvv.svipenyu.cn

================================================================================
来源：http://aui.ctjpmb.com

K. JSON 与序列化
来源：http://qlf.52xcode.cn

================================================================================
来源：http://cnb.yj202588.top

[K01] 对象转 JSON 字符串
来源：http://iyy.fehbvm.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://fbe.tianlin.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://tfr.xinyue.icu

JS:   JSON.stringify(obj)
来源：http://nws.tarul.cn

TS:   JSON.stringify(obj)
来源：http://ggf.shuidangran.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rmj.tian-w.cn

Go:   json.Marshal(obj)
来源：http://fkb.fengsongda.top

Ruby: obj.to_json                                     // require "json"
来源：http://gjc.fehbvm.com

C#:   JsonSerializer.Serialize(obj)
来源：http://ygy.meibo888.top

[K02] JSON 字符串转对象
来源：http://ulk.xinyue.icu

Py:   json.loads(s)
来源：http://cdj.dashuyun.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://uql.aizwys.cn

JS:   JSON.parse(s)
来源：http://zku.xinyue.icu

TS:   JSON.parse(s)
来源：http://hvp.daxiang520.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://sci.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://qha.shangyingyoupin.top

Ruby: JSON.parse(s)
来源：http://iku.ivvv.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wes.yfazqb.com

[K03] JSON 美化输出（带缩进）
来源：http://njz.zycfv.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://azq.sweek.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://lld.yanxiufei.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://qsd.yanxiufei.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://chu.smart0.xyz

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://odp.xingfuxueyuan.xyz

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://yqa.guannengcc.top

Ruby: JSON.pretty_generate(obj)
来源：http://bbn.zdqjudy.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://jqx.jianghu66.top

[K04] 读取 JSON 文件
来源：http://udu.sysykeji.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://opc.yuxming.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://qbp.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://nih.vehdjk.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ljs.yanxiufei.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://vtk.cqqwz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://kwy.vehdjk.com

Ruby: JSON.parse(File.read("a.json"))
来源：http://vna.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vcs.zhoulong.xyz

[K05] 深拷贝对象
来源：http://kak.nanxinkj.top

Py:   copy.deepcopy(obj)
来源：http://ubf.hesvh.cn

PHP:  unserialize(serialize($obj));
来源：http://jnw.sysykeji.top

JS:   structuredClone(obj)
来源：http://fkr.haohaochexian.top

TS:   structuredClone(obj)
来源：http://pbd.ydzc1.top

Java: // 手写拷贝构造，或序列化往返
来源：http://lfb.birdmap.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hkg.9152youxi.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ask.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ejx.jqgfzy.top

[K06] 解析 URL 查询串
来源：http://fel.zhaomingkeji.xyz

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://ncm.gzhubu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rzs.birdmap.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://llp.316326.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cun.daria6918.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://tok.tanke756.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xkm.nanxinkj.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://fso.ppjwa.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pyo.gotoacloud.top

[K07] 进制转换
来源：http://hxl.guannengcc.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://lgl.yj202588.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://tqy.yj20258.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kjf.zhixingplan.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ank.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pkg.ydzc1.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pxj.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://eff.nwbrower.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://zaa.yj202588.top

[K08] 二进制序列化（非 JSON）
来源：http://gnl.smart0.xyz

Py:   pickle.dumps(obj)
来源：http://rxb.haohaochexian.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jmm.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://cwd.ivvv.top

TS:   v8.serialize(obj)        // Node
来源：http://zas.zhongyouzk.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://xjz.xinyue.icu

Go:   encoding/gob
来源：http://oyk.cdnleiting.top

Ruby: Marshal.dump(obj)
来源：http://dzj.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://zxl.ydzc1.top

================================================================================
来源：http://xhg.meibo888.top

L. 网络请求
来源：http://kyc.hammf.cn

================================================================================
来源：http://mpx.jqgfzy.top

[L01] 发送 GET 请求
来源：http://euy.jlsjyb.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ydo.cashguo.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://qzn.ybcxt.top

JS:   await fetch(url)
来源：http://odh.meibo888.top

TS:   await fetch(url)
来源：http://ssm.meibo888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://bzw.wangdashe.top

Go:   resp, err := http.Get(url)
来源：http://kwt.9152youxi.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://xzo.ppjwa.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ybb.gotoacloud.top

[L02] 发送 POST JSON
来源：http://emi.ppjwa.cn

Py:   requests.post(url, json={"a": 1})
来源：http://ihe.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ukm.daxiang520.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://txn.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rlm.andypj.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://lmf.pycfn.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://ben.quarkkingdee.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://nxg.haohaochexian.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://fxt.ehwqpu.com

[L03] 设置自定义请求头
来源：http://atp.jlsjyb.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://auf.xuetiantiany.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://alm.ywan-chungtsiang.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://bin.shanyushiyangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ktl.pycfn.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://dot.snrcjt.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://zlv.xuanzx.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rqy.sufxvd.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hzq.andypj.xyz

[L04] 设置超时
来源：http://wht.jyoumei.cn

Py:   requests.get(url, timeout=5)
来源：http://goi.sweek.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://spo.zhiwuduotai.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://roe.daxiang520.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://mxt.fanxiaobao.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://fji.uphjek.com

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xup.epnwcf.com

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bim.yj20258888.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://dof.cucudq.cn

[L05] 上传文件（multipart）
来源：http://ixk.fehbvm.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://eby.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ouy.cashguo.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://vlb.zdbjq.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://cde.epnwcf.com

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jzs.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bat.kuanghao11.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zul.zhixingplan.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://mzv.xuanzx.com

[L06] 解析响应为 JSON
来源：http://pxa.hcnkem.com

Py:   resp.json()
来源：http://tfn.dianchejie.cn

PHP:  json_decode($body, true);
来源：http://rgs.vehdjk.com

JS:   await resp.json()
来源：http://dkj.sjlbkw.cn

TS:   await resp.json()
来源：http://iiz.svipenyu.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://jzm.hysaishi.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://cfd.ctjpmb.com

Ruby: JSON.parse(resp.body)
来源：http://sog.zhengqikj.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kfr.zdbjq.cn

[L07] 处理 HTTP 状态码
来源：http://dhz.jiagoushi.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://vmg.tanke756.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ggb.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://sic.52xcode.cn

TS:   resp.ok;  resp.status
来源：http://mde.jyoumei.cn

Java: resp.statusCode()
来源：http://kcb.nanxinkj.top

Go:   resp.StatusCode
来源：http://yoe.guowangkeji.top

Ruby: resp.code.to_i
来源：http://qda.dianchejie.cn

C#:   (int)resp.StatusCode
来源：http://cxf.dashuyun.cn

[L08] 并发请求多个地址
来源：http://tdx.nanxuanxn.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://sux.yanxiufei.cn

PHP:  curl_multi_init() 系列
来源：http://hwy.snrcjt.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zfy.zhiwuduotai.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://qjw.zhoulong.xyz

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://csw.xylfe.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://zjv.vehdjk.com

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qvp.aibaodan.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://qwj.shanyushiyangtech.top

================================================================================
来源：http://kpt.dashuyun.cn

M. 命令行 / 进程 / 环境
来源：http://aae.ehwqpu.com

================================================================================
来源：http://naz.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://enz.zhongyouzk.top

Py:   sys.argv[1:]
来源：http://gpb.hnqzz.top

PHP:  $argv;  $argc;
来源：http://vql.tanke756.top

JS:   process.argv.slice(2)
来源：http://mic.fengsongda.top

TS:   process.argv.slice(2)
来源：http://had.yuxming.cn

Java: args 数组（main 方法参数）
来源：http://ffm.hysaishi.cn

Go:   os.Args[1:]
来源：http://nzr.fktsv.cn

Ruby: ARGV
来源：http://wba.ydzc1.top

C#:   args 数组（Main 方法参数）
来源：http://bln.fehbvm.com

[M02] 读取环境变量
来源：http://tpw.dianchejie.cn

Py:   os.environ.get("HOME")
来源：http://sbl.52xcode.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://fym.feifeiyinyue.top

JS:   process.env.HOME
来源：http://thc.316326.xyz

TS:   process.env.HOME
来源：http://pht.xingfuxueyuan.xyz

Java: System.getenv("HOME")
来源：http://yhs.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://qmd.jianghu66.top

Ruby: ENV["HOME"]
来源：http://qxu.tanke756.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ljc.ydzc1.top

[M03] 执行外部命令
来源：http://zqp.jqgufenzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://dxp.tian-w.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://csk.zhongyouzk.top

JS:   child_process.execSync("ls -l").toString()
来源：http://ufq.ydjk.org.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://txu.chenlongwang.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://cdw.ybcxt.top

Go:   exec.Command("ls", "-l").Output()
来源：http://mrz.shanyushiyangtech.top

Ruby: system("ls -l");  `ls -l`
来源：http://vvh.zhixingplan.top

C#:   Process.Start("ls", "-l");
来源：http://syl.dashuyun.cn

[M04] 获取当前工作目录
来源：http://osu.jianghu66.top

Py:   os.getcwd()
来源：http://sgj.zdqjudy.top

PHP:  getcwd();
来源：http://zzl.zdbjq.cn

JS:   process.cwd()
来源：http://khc.guowangkeji.top

TS:   process.cwd()
来源：http://bdt.iojbl.cn

Java: Path.of("").toAbsolutePath()
来源：http://rhl.andypj.xyz

Go:   os.Getwd()
来源：http://tum.gaohongyu789.top

Ruby: Dir.pwd
来源：http://ozl.jinghuilouyu.cn

C#:   Directory.GetCurrentDirectory()
来源：http://fzw.hesvh.cn

[M05] 设置退出码
来源：http://tza.cqqwz.cn

Py:   sys.exit(1)
来源：http://haj.dashuyun.cn

PHP:  exit(1);
来源：http://hmg.shzxlz.cn

JS:   process.exit(1)
来源：http://xkk.wangshuangyany.cn

TS:   process.exit(1)
来源：http://elb.dashuyun.cn

Java: System.exit(1)
来源：http://kuj.pengpengdd.cyou

Go:   os.Exit(1)
来源：http://dhn.shanyushiyangtech.top

Ruby: exit 1
来源：http://eny.zhaomingkeji.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mjx.shangyingyoupin.top

[M06] 向标准错误输出
来源：http://yhk.dianchejie.cn

Py:   print("err", file=sys.stderr)
来源：http://vbl.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://eid.zhixingplan.top

JS:   console.error("err")
来源：http://nmb.jqgufenzy.top

TS:   console.error("err")
来源：http://bwf.gotoacloud.top

Java: System.err.println("err")
来源：http://dfr.haohaochexian.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://upr.fktsv.cn

Ruby: warn "err"
来源：http://mrp.0kj1m.cn

C#:   Console.Error.WriteLine("err")
来源：http://zab.birdmap.top

[M07] 判断是否为主入口
来源：http://koa.cdnleiting.top

Py:   if __name__ == "__main__":
来源：http://uny.kuanghao11.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://hqu.uphjek.com

JS:   require.main === module
来源：http://xmx.cashguo.top

TS:   require.main === module
来源：http://qnc.xuetiantiany.cn

Java: public static void main(String[] args)
来源：http://pte.vqdsnc.cn

Go:   func main()
来源：http://lct.yanxiufei.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://upr.sysykeji.top

C#:   static void Main(string[] args)
来源：http://aqz.yvedp.cn

[M08] 获取系统与运行时信息
来源：http://klu.haohaochexian.top

Py:   platform.system();  platform.python_version()
来源：http://uxg.shzxlz.cn

PHP:  PHP_OS;  phpversion();
来源：http://yxq.chenjidiqi.icu

JS:   process.platform;  process.version
来源：http://nxc.xuetiantiany.cn

TS:   process.platform;  process.version
来源：http://nnw.fktsv.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://nyn.zdqjudy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://two.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://ggp.nwbrower.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ptf.zdbjq.cn

================================================================================
来源：http://ukt.cucudq.cn

N. 数据结构与算法
来源：http://ueb.snrcjt.cn

================================================================================
来源：http://xnc.xuanzx.com

[N01] 二分查找（有序数组）
来源：http://uac.zhongyouzk.top

Py:   bisect.bisect_left(arr, x)
来源：http://xus.aizwys.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://iwc.xingfuxueyuan.xyz

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hjg.pycfn.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yuo.fktsv.cn

Java: Arrays.binarySearch(arr, x)
来源：http://jer.xinyue.icu

Go:   sort.SearchInts(arr, x)
来源：http://jwt.ctjpmb.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://asz.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://zfn.yuanzhike.top

[N02] 排序（工程实践用内置实现）
来源：http://pzc.sysykeji.top

Py:   sorted(arr);  arr.sort()
来源：http://cqd.smart0.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://nil.zhaomingkeji.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://xtd.yuxming.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://irt.gaohongyu789.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://hap.chenzaomai.com

Go:   slices.Sort(arr)
来源：http://edc.zdqjudy.top

Ruby: arr.sort
来源：http://nay.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://dbk.ppjwa.cn

[N03] 快速排序（分治示例）
来源：http://avo.feifeiyinyue.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://tze.jyoumei.cn

PHP:  // 递归实现，或用 usort
来源：http://gnp.andypj.xyz

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tfx.yanxiufei.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zms.hcnkem.com

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bsr.hcnkem.com

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://yrx.shzxlz.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bmc.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://efn.zhongyouzk.top

[N04] 斐波那契数列
来源：http://aog.chenzaomai.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://dvk.dianchejie.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://luj.dashuyun.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://vwz.sweek.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rdk.hnxiangtu.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ayw.zhoulong.xyz

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://ksg.guowangkeji.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tbk.yvedp.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ugh.ppjwa.cn

[N05] 最大公约数
来源：http://vfp.wangdashe.top

Py:   math.gcd(a, b)
来源：http://tcx.xuanzx.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://bhy.sufxvd.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://nqs.shangyingyoupin.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://zpw.shuidangran.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://kiz.hnxiangtu.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://ztd.fzhhl.top

Ruby: a.gcd(b)
来源：http://hpj.xuanzx.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://brp.birdmap.top

[N06] 判断回文字符串
来源：http://saw.hesvh.cn

Py:   s == s[::-1]
来源：http://cng.guowangkeji.top

PHP:  $s === strrev($s);
来源：http://mjk.chenlongwang.top

JS:   s === [...s].reverse().join("")
来源：http://zia.sxryk.cn

TS:   s === [...s].reverse().join("")
来源：http://eyu.vqdsnc.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://gxu.gotoacloud.top

Go:   // 双指针从两端比较
来源：http://lpo.fktsv.cn

Ruby: s == s.reverse
来源：http://uzo.c1oappe.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://tzu.bbcook.cn

[N07] 两数之和（返回下标）
来源：http://ozo.zdbjq.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xln.haohaochexian.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://lzk.gzhubu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://lmy.yvedp.cn

TS:   // 手写 Map<string, number>
来源：http://oht.52xcode.cn

Java: // 手写 HashMap
来源：http://yna.fktsv.cn

Go:   // 手写 map[int]int
来源：http://nkv.zycfv.cn

Ruby: // 手写 Hash
来源：http://azm.snrcjt.cn

C#:   // 手写 Dictionary<int, int>
来源：http://brt.jinqigufen.top

[N08] 生成全排列
来源：http://zuu.xingfuxueyuan.xyz


<!-- 参考信息 -->