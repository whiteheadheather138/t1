代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dxv.yj20258.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://quq.yj20258888.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://ijk.xinyue.icu

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xeh.gzhubu.top

================================================================================
来源：http://flu.hnqzz.top

K. JSON 与序列化
来源：http://zyl.sweek.top

================================================================================
来源：http://pnv.yanxiufei.cn

[K01] 对象转 JSON 字符串
来源：http://ysh.meibo888.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://usm.redwolf501.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://sub.zhaomingkeji.xyz

JS:   JSON.stringify(obj)
来源：http://ghc.shanyushiyangtech.top

TS:   JSON.stringify(obj)
来源：http://uwu.uphjek.com

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://ncb.zycfv.cn

Go:   json.Marshal(obj)
来源：http://xyt.jinqigufen.top

Ruby: obj.to_json                                     // require "json"
来源：http://ecl.bbcook.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://jan.bjfxy.top

[K02] JSON 字符串转对象
来源：http://ipi.wangdashe.top

Py:   json.loads(s)
来源：http://cxe.redwolf501.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://vrt.ywan-chungtsiang.top

JS:   JSON.parse(s)
来源：http://cex.9152youxi.cn

TS:   JSON.parse(s)
来源：http://nfp.sxryk.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://yej.pycfn.com

Go:   json.Unmarshal(data, &v)
来源：http://ryt.aibaodan.cn

Ruby: JSON.parse(s)
来源：http://wgn.hongshengwenyu.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ece.jinqigufen.top

[K03] JSON 美化输出（带缩进）
来源：http://vmz.aizwys.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://gom.fehbvm.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://scg.tian-w.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://gsb.0kj1m.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xhr.aizwys.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pmv.ctjpmb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xbh.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://all.vehdjk.com

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://hum.zhoulong.xyz

[K04] 读取 JSON 文件
来源：http://aqc.cashguo.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://cbl.redwolf501.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://xmb.jqgfzy.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kuo.nanxinkj.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jhy.cqqwz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://oxz.ehwqpu.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://okw.fzhhl.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://kcs.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rup.hnqzz.top

[K05] 深拷贝对象
来源：http://llk.shzxlz.cn

Py:   copy.deepcopy(obj)
来源：http://swr.ehwqpu.com

PHP:  unserialize(serialize($obj));
来源：http://ldw.yanxiufei.cn

JS:   structuredClone(obj)
来源：http://anb.vqdsnc.cn

TS:   structuredClone(obj)
来源：http://crh.vehdjk.com

Java: // 手写拷贝构造，或序列化往返
来源：http://owt.jyoumei.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://ukv.gzhubu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lsu.hfpthk.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://nmw.daxiang520.top

[K06] 解析 URL 查询串
来源：http://hev.ctjpmb.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://xhz.tianlin.xyz

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://wwv.xziqi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ncy.fengsongda.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ufl.hesvh.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://krt.fanxiaobao.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://zfs.meibo888.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gfj.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hqe.chenlongwang.top

[K07] 进制转换
来源：http://nmt.zdqjudy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mmr.zhiwuduotai.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://eli.hammf.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://utl.ybcxt.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ykx.hfpthk.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dfc.daxiang520.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ffq.aizwys.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://kjs.sufxvd.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uid.yanxiufei.cn

[K08] 二进制序列化（非 JSON）
来源：http://dbz.yongpay.top

Py:   pickle.dumps(obj)
来源：http://vpr.hnqzz.top

PHP:  serialize($obj);  unserialize($s);
来源：http://alz.cashguo.top

JS:   v8.serialize(obj)        // Node
来源：http://maq.fzhhl.top

TS:   v8.serialize(obj)        // Node
来源：http://ret.ybcxt.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dgn.feifeiyinyue.top

Go:   encoding/gob
来源：http://lbt.sweek.top

Ruby: Marshal.dump(obj)
来源：http://tsk.guannengcc.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://nqf.cashguo.top

================================================================================
来源：http://gnc.cdnleiting.top

L. 网络请求
来源：http://jws.chenjidiqi.icu

================================================================================
来源：http://cfz.cqqwz.cn

[L01] 发送 GET 请求
来源：http://oxj.aizwys.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://rcg.shuidangran.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://wii.yanxiufei.cn

JS:   await fetch(url)
来源：http://ove.jqgfzy.top

TS:   await fetch(url)
来源：http://ciw.ywan-chungtsiang.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://xly.0kj1m.cn

Go:   resp, err := http.Get(url)
来源：http://upt.fengsongda.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ycs.havefunace.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wml.bbcook.cn

[L02] 发送 POST JSON
来源：http://mfg.gogol.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://vap.jyoumei.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://pko.ctjpmb.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://crb.jyoumei.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://stl.chenjidiqi.icu

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ghf.hfpthk.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://vmf.sxryk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gmp.ppjwa.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://nyf.jinyuanbaomall.cn

[L03] 设置自定义请求头
来源：http://zko.chenlongwang.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://qdt.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fpl.ppjwa.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://pqe.xziqi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hlu.hnxiangtu.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ysc.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jnx.ydzc1.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://tgl.pengpengdd.cyou

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://dnf.xuetiantiany.cn

[L04] 设置超时
来源：http://hyn.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://wjl.xylfe.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uqr.shuidangran.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://yky.fengsongda.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ywc.yangfankeji.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://enl.nanxuanxn.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aqv.cheryme.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fgg.jinqigfzy.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://fmt.chenlongwang.top

[L05] 上传文件（multipart）
来源：http://mdk.52xcode.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tem.guowangkeji.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://noj.epnwcf.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://kts.yangfankeji.com

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://tms.yueranfly.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://qvc.shangyingyoupin.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://lhm.yuxming.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://usx.jyoumei.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dzp.meibo888.top

[L06] 解析响应为 JSON
来源：http://hhd.cucudq.cn

Py:   resp.json()
来源：http://jil.svipenyu.cn

PHP:  json_decode($body, true);
来源：http://xqd.aibaodan.cn

JS:   await resp.json()
来源：http://jkp.daria6918.cn

TS:   await resp.json()
来源：http://qto.hfpthk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://mdc.yj20258.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://nlb.feifeiyinyue.top

Ruby: JSON.parse(resp.body)
来源：http://kct.hywenlv.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xbw.yj20258.top

[L07] 处理 HTTP 状态码
来源：http://shf.ctjpmb.com

Py:   resp.status_code;  resp.raise_for_status()
来源：http://lkq.wangshuangyany.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://umn.cdnleiting.top

JS:   resp.ok;  resp.status
来源：http://tem.316326.xyz

TS:   resp.ok;  resp.status
来源：http://tba.tarul.cn

Java: resp.statusCode()
来源：http://jfj.zhiwuduotai.top

Go:   resp.StatusCode
来源：http://zzu.hcnkem.com

Ruby: resp.code.to_i
来源：http://lrp.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://mlq.havefunace.top

[L08] 并发请求多个地址
来源：http://fet.epnwcf.com

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://uql.9152youxi.cn

PHP:  curl_multi_init() 系列
来源：http://ndw.yj202588.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://zko.hywenlv.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://dlh.ppjwa.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://lwa.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wzl.redwolf501.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://tdx.zhaomingkeji.xyz

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ucr.cdnleiting.top

================================================================================
来源：http://fyu.gotoacloud.top

M. 命令行 / 进程 / 环境
来源：http://uhm.yuxming.cn

================================================================================
来源：http://ymz.hesvh.cn

[M01] 读取命令行参数
来源：http://boo.fehbvm.com

Py:   sys.argv[1:]
来源：http://bpw.guowangkeji.top

PHP:  $argv;  $argc;
来源：http://jwz.bbcook.cn

JS:   process.argv.slice(2)
来源：http://dvy.dashuyun.cn

TS:   process.argv.slice(2)
来源：http://ype.ehwqpu.com

Java: args 数组（main 方法参数）
来源：http://kbo.jiagoushi.top

Go:   os.Args[1:]
来源：http://ebg.shanyushiyangtech.top

Ruby: ARGV
来源：http://enx.mhx1999.top

C#:   args 数组（Main 方法参数）
来源：http://wlz.fanxiaobao.xyz

[M02] 读取环境变量
来源：http://bxi.yfazqb.com

Py:   os.environ.get("HOME")
来源：http://rmu.zhijiandao.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://gun.ydjk.org.cn

JS:   process.env.HOME
来源：http://ubp.haohaochexian.top

TS:   process.env.HOME
来源：http://waz.sufxvd.cn

Java: System.getenv("HOME")
来源：http://aqd.fktsv.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://szo.bjfxy.top

Ruby: ENV["HOME"]
来源：http://dqf.guannengcc.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://jeh.zhongyouzk.top

[M03] 执行外部命令
来源：http://one.zhijiandao.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ili.yfazqb.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://xug.jyoumei.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://ixm.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://tem.yuxming.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://mnk.yj202588.top

Go:   exec.Command("ls", "-l").Output()
来源：http://dfr.tanke756.top

Ruby: system("ls -l");  `ls -l`
来源：http://xjk.yj20258888.top

C#:   Process.Start("ls", "-l");
来源：http://vgc.ydjk.org.cn

[M04] 获取当前工作目录
来源：http://enn.gaohongyu789.top

Py:   os.getcwd()
来源：http://qzz.jqgufenzy.top

PHP:  getcwd();
来源：http://xqa.nanxinkj.top

JS:   process.cwd()
来源：http://koy.jianghu66.top

TS:   process.cwd()
来源：http://jui.ybcxt.top

Java: Path.of("").toAbsolutePath()
来源：http://gdz.tanke756.top

Go:   os.Getwd()
来源：http://jxl.cucudq.cn

Ruby: Dir.pwd
来源：http://wak.andypj.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://wqp.zhixingplan.top

[M05] 设置退出码
来源：http://kxk.gogol.net.cn

Py:   sys.exit(1)
来源：http://iur.jlsjyb.cn

PHP:  exit(1);
来源：http://qxo.fktsv.cn

JS:   process.exit(1)
来源：http://vnr.iojbl.cn

TS:   process.exit(1)
来源：http://nsd.meibo888.top

Java: System.exit(1)
来源：http://vlg.ctjpmb.com

Go:   os.Exit(1)
来源：http://nsh.jqgufenzy.top

Ruby: exit 1
来源：http://ndo.xuanzx.com

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://wxg.yonumen.top

[M06] 向标准错误输出
来源：http://hon.jinghuilouyu.cn

Py:   print("err", file=sys.stderr)
来源：http://iti.meibo888.top

PHP:  fwrite(STDERR, "err\n");
来源：http://rqs.0kj1m.cn

JS:   console.error("err")
来源：http://epl.sxryk.cn

TS:   console.error("err")
来源：http://dex.yj20258888.top

Java: System.err.println("err")
来源：http://bqe.zhoulong.xyz

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hvk.xylfe.cn

Ruby: warn "err"
来源：http://idi.zhongyouzk.top

C#:   Console.Error.WriteLine("err")
来源：http://hrz.jinyuanbaomall.cn

[M07] 判断是否为主入口
来源：http://kqi.fehbvm.com

Py:   if __name__ == "__main__":
来源：http://yge.chenjidiqi.icu

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jtf.zhixingplan.top

JS:   require.main === module
来源：http://fur.gogol.net.cn

TS:   require.main === module
来源：http://ihr.jiagoushi.top

Java: public static void main(String[] args)
来源：http://gze.hywenlv.cn

Go:   func main()
来源：http://eer.gaohongyu789.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://dck.cqqwz.cn

C#:   static void Main(string[] args)
来源：http://rnd.aizwys.cn

[M08] 获取系统与运行时信息
来源：http://cql.52xcode.cn

Py:   platform.system();  platform.python_version()
来源：http://taj.cdnleiting.top

PHP:  PHP_OS;  phpversion();
来源：http://eey.cheryme.top

JS:   process.platform;  process.version
来源：http://ddl.mhx1999.top

TS:   process.platform;  process.version
来源：http://ikv.snrcjt.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hzt.shanyushiyangkeji.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://sie.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://vwx.aibaodan.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://wyi.haohaochexian.top

================================================================================
来源：http://gct.andypj.xyz

N. 数据结构与算法
来源：http://frr.tian-w.cn

================================================================================
来源：http://kll.xylfe.cn

[N01] 二分查找（有序数组）
来源：http://lyq.feifeiyinyue.top

Py:   bisect.bisect_left(arr, x)
来源：http://ivj.zhongyouzk.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pia.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://htu.zhaomingkeji.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hzk.yvedp.cn

Java: Arrays.binarySearch(arr, x)
来源：http://via.quarkkingdee.top

Go:   sort.SearchInts(arr, x)
来源：http://kqf.yueranfly.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://fwd.ctjpmb.com

C#:   Array.BinarySearch(arr, x)
来源：http://yoc.meibo888.top

[N02] 排序（工程实践用内置实现）
来源：http://hqi.quarkkingdee.top

Py:   sorted(arr);  arr.sort()
来源：http://uic.andypj.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://qqz.ybcxt.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://sed.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://lin.cdnleiting.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cpz.jyoumei.cn

Go:   slices.Sort(arr)
来源：http://vdr.pengpengdd.cyou

Ruby: arr.sort
来源：http://xew.meibo888.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://jxx.feifeiyinyue.top

[N03] 快速排序（分治示例）
来源：http://met.yvedp.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://xlk.ivvv.top

PHP:  // 递归实现，或用 usort
来源：http://mjs.yongpay.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://tdd.ydjk.org.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zwh.c1oappe.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://szp.sysykeji.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ohi.yonumen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://brl.chenzaomai.com

C#:   // 手写递归，或 Array.Sort
来源：http://qwy.meibo888.top

[N04] 斐波那契数列
来源：http://wnh.pengpengdd.cyou

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yul.sysykeji.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://ilj.ppjwa.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://lcq.ppjwa.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://mnu.aibaodan.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://nhy.yvedp.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://dya.quarkkingdee.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ixm.ydzc1.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://pbg.jinqigufen.top

[N05] 最大公约数
来源：http://hwp.birdmap.top

Py:   math.gcd(a, b)
来源：http://xjv.hcnkem.com

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fpp.yueranfly.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://xef.cqqwz.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lop.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ioe.vehdjk.com

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pvc.birdmap.top

Ruby: a.gcd(b)
来源：http://tde.9152youxi.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dbn.andypj.xyz

[N06] 判断回文字符串
来源：http://wvh.smart0.xyz

Py:   s == s[::-1]
来源：http://mis.sxryk.cn

PHP:  $s === strrev($s);
来源：http://myi.yangfankeji.com

JS:   s === [...s].reverse().join("")
来源：http://mpl.gogol.net.cn

TS:   s === [...s].reverse().join("")
来源：http://jjq.yvedp.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://uce.quarkkingdee.top

Go:   // 双指针从两端比较
来源：http://xmv.yanxiufei.cn

Ruby: s == s.reverse
来源：http://pyw.gogol.net.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cgr.fanxiaobao.xyz

[N07] 两数之和（返回下标）
来源：http://ble.shzxlz.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://bsn.havefunace.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qjj.xylfe.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://gdm.jinyuanbaomall.cn

TS:   // 手写 Map<string, number>
来源：http://tsm.zhoulong.xyz

Java: // 手写 HashMap
来源：http://ele.havefunace.top

Go:   // 手写 map[int]int
来源：http://qjb.chenjidiqi.icu

Ruby: // 手写 Hash
来源：http://ejx.aibaodan.cn

C#:   // 手写 Dictionary<int, int>
来源：http://nnc.gotoacloud.top

[N08] 生成全排列
来源：http://jae.xziqi.cn

Py:   itertools.permutations(arr)
来源：http://mmx.andypj.xyz

PHP:  // 手写递归交换
来源：http://znn.vehdjk.com

JS:   // 手写回溯递归
来源：http://jnp.zhiwuduotai.top

TS:   // 手写回溯递归
来源：http://raa.yvedp.cn


<!-- 参考信息 -->