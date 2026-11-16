代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wyn.iojbl.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://lkj.cdnleiting.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://mlp.zhongyouzk.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://owo.iojbl.cn

================================================================================
来源：http://erv.zdqjudy.top

K. JSON 与序列化
来源：http://daj.0kj1m.cn

================================================================================
来源：http://nkd.xinyue.icu

[K01] 对象转 JSON 字符串
来源：http://qdl.daxiang520.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://qrt.zhaomingkeji.xyz

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://blx.yj20258888.top

JS:   JSON.stringify(obj)
来源：http://ahn.hnxiangtu.top

TS:   JSON.stringify(obj)
来源：http://fsc.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://chl.zdbjq.cn

Go:   json.Marshal(obj)
来源：http://moh.zhaomingkeji.xyz

Ruby: obj.to_json                                     // require "json"
来源：http://pkd.guowangkeji.top

C#:   JsonSerializer.Serialize(obj)
来源：http://afy.hongshengwenyu.top

[K02] JSON 字符串转对象
来源：http://xzc.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://fhe.xingfuxueyuan.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cut.gaohongyu789.top

JS:   JSON.parse(s)
来源：http://qls.jinqigufen.top

TS:   JSON.parse(s)
来源：http://kuu.chenjidiqi.icu

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://uxa.xingfuxueyuan.xyz

Go:   json.Unmarshal(data, &v)
来源：http://pnk.redwolf501.top

Ruby: JSON.parse(s)
来源：http://hlv.jqgfzy.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://hbo.iojbl.cn

[K03] JSON 美化输出（带缩进）
来源：http://faw.gaohongyu789.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tcw.tianlin.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://tlf.epnwcf.com

JS:   JSON.stringify(obj, null, 2)
来源：http://vyd.hnqzz.top

TS:   JSON.stringify(obj, null, 2)
来源：http://tej.zhongyouzk.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rub.yuanzhike.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://gvp.aizwys.cn

Ruby: JSON.pretty_generate(obj)
来源：http://gke.shanyushiyangtech.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://iiz.jianghu66.top

[K04] 读取 JSON 文件
来源：http://kbb.hnqzz.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qff.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://dwl.0kj1m.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://znv.gzhubu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://aws.tianlin.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://qdb.yongpay.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://opk.bbcook.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://chz.bbcook.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://rif.fzhhl.top

[K05] 深拷贝对象
来源：http://acq.hesvh.cn

Py:   copy.deepcopy(obj)
来源：http://bdc.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://ncm.jqgfzy.top

JS:   structuredClone(obj)
来源：http://akm.gotoacloud.top

TS:   structuredClone(obj)
来源：http://cmr.yj202588.top

Java: // 手写拷贝构造，或序列化往返
来源：http://gjf.daxiang520.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://crh.cheryme.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nuh.zdbjq.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://wuu.quarkkingdee.top

[K06] 解析 URL 查询串
来源：http://nor.meibo888.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://fiq.aizwys.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://lzv.dashuyun.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gco.dashuyun.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ufo.guowangkeji.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://bow.chenjidiqi.icu

Go:   url.ParseQuery("a=1&b=2")
来源：http://xzw.cucudq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://hei.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://hnt.shangyingyoupin.top

[K07] 进制转换
来源：http://rov.yueranfly.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hpr.feifeiyinyue.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://str.zhaomingkeji.xyz

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://koo.gzhubu.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://rtb.dianchejie.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://pty.jiagoushi.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://aqn.bjfxy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lcs.jqgfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://geo.xingfuxueyuan.xyz

[K08] 二进制序列化（非 JSON）
来源：http://uer.yvedp.cn

Py:   pickle.dumps(obj)
来源：http://ymx.ivvv.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dox.vqdsnc.cn

JS:   v8.serialize(obj)        // Node
来源：http://rec.cucudq.cn

TS:   v8.serialize(obj)        // Node
来源：http://bze.gogol.net.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kox.tian-w.cn

Go:   encoding/gob
来源：http://rcc.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://zsa.jianghu66.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mns.quarkkingdee.top

================================================================================
来源：http://oht.cashguo.top

L. 网络请求
来源：http://xzv.zdqjudy.top

================================================================================
来源：http://mcw.bbcook.cn

[L01] 发送 GET 请求
来源：http://xon.gzhubu.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://mvz.jqgufenzy.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://uhi.shzxlz.cn

JS:   await fetch(url)
来源：http://xxu.0kj1m.cn

TS:   await fetch(url)
来源：http://jlk.9152youxi.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://erh.fzhhl.top

Go:   resp, err := http.Get(url)
来源：http://jfl.tanke756.top

Ruby: Net::HTTP.get(URI(url))
来源：http://kav.aizwys.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://khf.havefunace.top

[L02] 发送 POST JSON
来源：http://pdx.shuidangran.top

Py:   requests.post(url, json={"a": 1})
来源：http://udi.aibaodan.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://grd.birdmap.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://skg.birdmap.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dvu.guannengcc.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nov.gaohongyu789.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://kdz.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gvr.sxryk.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://inn.fehbvm.com

[L03] 设置自定义请求头
来源：http://mzu.zhijiandao.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pbq.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://sre.sufxvd.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://wze.guowangkeji.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ylo.shuidangran.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qvb.c1oappe.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://jre.fengsongda.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://odq.sweek.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://mib.cashguo.top

[L04] 设置超时
来源：http://uae.yj20258.top

Py:   requests.get(url, timeout=5)
来源：http://zym.andypj.xyz

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ifw.sjlbkw.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ile.0kj1m.cn

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://hyu.yonumen.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://opg.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://bhn.chenlongwang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://pim.yj20258.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rqv.ivvv.top

[L05] 上传文件（multipart）
来源：http://xiw.zhongyouzk.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://tvx.snrcjt.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://zzv.hammf.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wez.wangshuangyany.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gpk.0kj1m.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://crj.hcnkem.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xjj.zhijiandao.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zbi.yonumen.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://gkr.hammf.cn

[L06] 解析响应为 JSON
来源：http://fhr.tanke756.top

Py:   resp.json()
来源：http://siq.hcnkem.com

PHP:  json_decode($body, true);
来源：http://hrz.xuetiantiany.cn

JS:   await resp.json()
来源：http://wut.wangdashe.top

TS:   await resp.json()
来源：http://yzl.sxryk.cn

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://zoo.uphjek.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://vmc.jinqigfzy.top

Ruby: JSON.parse(resp.body)
来源：http://lhh.meibo888.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ltj.hcnkem.com

[L07] 处理 HTTP 状态码
来源：http://yzn.yueranfly.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://qmm.fengsongda.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://vlf.chenzaomai.com

JS:   resp.ok;  resp.status
来源：http://xhv.epnwcf.com

TS:   resp.ok;  resp.status
来源：http://zsd.cdnleiting.top

Java: resp.statusCode()
来源：http://cak.hammf.cn

Go:   resp.StatusCode
来源：http://mpx.yuanzhike.top

Ruby: resp.code.to_i
来源：http://jwh.sweek.top

C#:   (int)resp.StatusCode
来源：http://cxd.bbcook.cn

[L08] 并发请求多个地址
来源：http://uhw.jinqigufen.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://tpg.wangshuangyany.cn

PHP:  curl_multi_init() 系列
来源：http://cut.sxryk.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://lqq.redwolf501.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://jam.quarkkingdee.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://mow.ybcxt.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vpj.gzhubu.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://cdh.sxryk.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://clh.smart0.xyz

================================================================================
来源：http://koz.sjlbkw.cn

M. 命令行 / 进程 / 环境
来源：http://baj.yvedp.cn

================================================================================
来源：http://wyq.xylfe.cn

[M01] 读取命令行参数
来源：http://yvw.aizwys.cn

Py:   sys.argv[1:]
来源：http://wib.haohaochexian.top

PHP:  $argv;  $argc;
来源：http://haw.zhiwuduotai.top

JS:   process.argv.slice(2)
来源：http://xll.birdmap.top

TS:   process.argv.slice(2)
来源：http://qqn.zhongyouzk.top

Java: args 数组（main 方法参数）
来源：http://ydo.zhijiandao.cn

Go:   os.Args[1:]
来源：http://lmx.pycfn.com

Ruby: ARGV
来源：http://hez.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://ahp.jqgufenzy.top

[M02] 读取环境变量
来源：http://kth.hysaishi.cn

Py:   os.environ.get("HOME")
来源：http://mrn.daxiang520.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pgs.dashuyun.cn

JS:   process.env.HOME
来源：http://wbg.jqgfzy.top

TS:   process.env.HOME
来源：http://izc.jiagoushi.top

Java: System.getenv("HOME")
来源：http://hwk.chenjidiqi.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://tgg.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://xct.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://igj.yfazqb.com

[M03] 执行外部命令
来源：http://xym.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://gko.chenzaomai.com

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://mcb.tian-w.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://zgc.yvedp.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ztb.wangshuangyany.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://gbt.jiagoushi.top

Go:   exec.Command("ls", "-l").Output()
来源：http://hqh.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://yjm.jqgufenzy.top

C#:   Process.Start("ls", "-l");
来源：http://xgp.tian-w.cn

[M04] 获取当前工作目录
来源：http://xui.aizwys.cn

Py:   os.getcwd()
来源：http://anv.hammf.cn

PHP:  getcwd();
来源：http://ioc.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://gob.cqqwz.cn

TS:   process.cwd()
来源：http://qts.9152youxi.cn

Java: Path.of("").toAbsolutePath()
来源：http://mic.nanxuanxn.top

Go:   os.Getwd()
来源：http://apn.smart0.xyz

Ruby: Dir.pwd
来源：http://cvm.xuanzx.com

C#:   Directory.GetCurrentDirectory()
来源：http://gue.jlsjyb.cn

[M05] 设置退出码
来源：http://tgm.pengpengdd.cyou

Py:   sys.exit(1)
来源：http://dpo.nanxuanxn.top

PHP:  exit(1);
来源：http://cdp.chenzaomai.com

JS:   process.exit(1)
来源：http://ntn.yuanzhike.top

TS:   process.exit(1)
来源：http://kzt.uphjek.com

Java: System.exit(1)
来源：http://xdp.jyoumei.cn

Go:   os.Exit(1)
来源：http://hsx.ivvv.top

Ruby: exit 1
来源：http://xed.fanxiaobao.xyz

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pyl.dianchejie.cn

[M06] 向标准错误输出
来源：http://lcr.havefunace.top

Py:   print("err", file=sys.stderr)
来源：http://tun.vqdsnc.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://knk.yonumen.top

JS:   console.error("err")
来源：http://uko.fengsongda.top

TS:   console.error("err")
来源：http://hox.mhx1999.top

Java: System.err.println("err")
来源：http://dfd.gogol.net.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://wvt.nanxuanxn.top

Ruby: warn "err"
来源：http://ide.9152youxi.cn

C#:   Console.Error.WriteLine("err")
来源：http://dyt.yuanzhike.top

[M07] 判断是否为主入口
来源：http://xrb.zhengqikj.top

Py:   if __name__ == "__main__":
来源：http://bmq.tanke756.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gul.feifeiyinyue.top

JS:   require.main === module
来源：http://fla.pycfn.com

TS:   require.main === module
来源：http://tlz.jqgfzy.top

Java: public static void main(String[] args)
来源：http://cgy.316326.xyz

Go:   func main()
来源：http://xuo.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://gqk.jlsjyb.cn

C#:   static void Main(string[] args)
来源：http://avu.fktsv.cn

[M08] 获取系统与运行时信息
来源：http://mqy.jinyuanbaomall.cn

Py:   platform.system();  platform.python_version()
来源：http://bcr.sjlbkw.cn

PHP:  PHP_OS;  phpversion();
来源：http://tol.0kj1m.cn

JS:   process.platform;  process.version
来源：http://squ.bjfxy.top

TS:   process.platform;  process.version
来源：http://fuw.yj20258.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://wby.zhongyouzk.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://bru.dashuyun.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://noz.yj20258888.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://ubx.wangshuangyany.cn

================================================================================
来源：http://fwm.ctjpmb.com

N. 数据结构与算法
来源：http://snh.sysykeji.top

================================================================================
来源：http://adj.guowangkeji.top

[N01] 二分查找（有序数组）
来源：http://yzm.hnqzz.top

Py:   bisect.bisect_left(arr, x)
来源：http://isd.yj20258.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://awa.zycfv.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ore.ybcxt.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://jhv.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://rzx.yfazqb.com

Go:   sort.SearchInts(arr, x)
来源：http://fqf.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://wpv.nanxuanxn.top

C#:   Array.BinarySearch(arr, x)
来源：http://scr.wangdashe.top

[N02] 排序（工程实践用内置实现）
来源：http://wyj.ydzc1.top

Py:   sorted(arr);  arr.sort()
来源：http://brc.fanxiaobao.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://xxr.sxryk.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://dut.smart0.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://ecr.zhixingplan.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://vxt.smart0.xyz

Go:   slices.Sort(arr)
来源：http://iko.quarkkingdee.top

Ruby: arr.sort
来源：http://olx.sufxvd.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://ldr.ppjwa.cn

[N03] 快速排序（分治示例）
来源：http://dim.jiagoushi.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://sep.ppjwa.cn

PHP:  // 递归实现，或用 usort
来源：http://sty.chenzaomai.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://akt.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hkm.tianlin.xyz

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ksi.svipenyu.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://kya.zhixingplan.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://itp.xuanzx.com

C#:   // 手写递归，或 Array.Sort
来源：http://rlj.fehbvm.com

[N04] 斐波那契数列
来源：http://yzt.birdmap.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wuk.iojbl.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://svg.yonumen.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ddd.nanxinkj.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rin.hcnkem.com

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ahb.sjlbkw.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://rga.feifeiyinyue.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iok.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://vpi.gogol.net.cn

[N05] 最大公约数
来源：http://dtx.cucudq.cn

Py:   math.gcd(a, b)
来源：http://klk.sjlbkw.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://adk.jinghuilouyu.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ytl.havefunace.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://obg.zhengqikj.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wum.ydzc1.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://wdq.hammf.cn

Ruby: a.gcd(b)
来源：http://gtj.316326.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://qjv.sxryk.cn

[N06] 判断回文字符串
来源：http://vfg.feifeiyinyue.top

Py:   s == s[::-1]
来源：http://qeb.tarul.cn

PHP:  $s === strrev($s);
来源：http://aoe.smart0.xyz

JS:   s === [...s].reverse().join("")
来源：http://lgt.zdbjq.cn

TS:   s === [...s].reverse().join("")
来源：http://kib.fanxiaobao.xyz

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://aau.tian-w.cn

Go:   // 双指针从两端比较
来源：http://qjn.sxryk.cn

Ruby: s == s.reverse
来源：http://aoz.vehdjk.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://ssj.meibo888.top

[N07] 两数之和（返回下标）
来源：http://qjj.xuanzx.com

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://edo.gaohongyu789.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://qex.hysaishi.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://svj.52xcode.cn

TS:   // 手写 Map<string, number>
来源：http://xcu.ydzc1.top

Java: // 手写 HashMap
来源：http://nso.316326.xyz

Go:   // 手写 map[int]int
来源：http://slb.jinghuilouyu.cn

Ruby: // 手写 Hash
来源：http://zeh.chenzaomai.com

C#:   // 手写 Dictionary<int, int>
来源：http://bpj.sjlbkw.cn

[N08] 生成全排列
来源：http://kjv.nanxinkj.top

Py:   itertools.permutations(arr)
来源：http://ezr.sweek.top

PHP:  // 手写递归交换
来源：http://khz.fehbvm.com

JS:   // 手写回溯递归
来源：http://smk.jlsjyb.cn

TS:   // 手写回溯递归
来源：http://sqq.xuanzx.com


<!-- 参考信息 -->