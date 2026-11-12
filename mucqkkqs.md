代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://jpp.tian-w.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://xbw.kuanghao11.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://qyk.daxiang520.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xuf.havefunace.top

================================================================================
来源：http://gcb.zdqjudy.top

K. JSON 与序列化
来源：http://yql.redwolf501.top

================================================================================
来源：http://xld.jinqigufen.top

[K01] 对象转 JSON 字符串
来源：http://fer.xziqi.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jbf.ydjk.org.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://gkj.smart0.xyz

JS:   JSON.stringify(obj)
来源：http://twx.aizwys.cn

TS:   JSON.stringify(obj)
来源：http://nqu.jiagoushi.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://xco.yj202588.top

Go:   json.Marshal(obj)
来源：http://oko.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://lou.hammf.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://tuo.gogol.net.cn

[K02] JSON 字符串转对象
来源：http://rgs.fzhhl.top

Py:   json.loads(s)
来源：http://ytf.hcnkem.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lqe.pycfn.com

JS:   JSON.parse(s)
来源：http://wjq.hesvh.cn

TS:   JSON.parse(s)
来源：http://kzt.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://kco.ivvv.top

Go:   json.Unmarshal(data, &v)
来源：http://bpa.yfazqb.com

Ruby: JSON.parse(s)
来源：http://wdk.svipenyu.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://yos.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://nbw.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xhq.xinyue.icu

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ure.jlsjyb.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jtx.nanxuanxn.top

TS:   JSON.stringify(obj, null, 2)
来源：http://prs.guannengcc.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://nms.52xcode.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://tjy.pengpengdd.cyou

Ruby: JSON.pretty_generate(obj)
来源：http://ovz.tianlin.xyz

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://sfi.xuetiantiany.cn

[K04] 读取 JSON 文件
来源：http://duh.kuanghao11.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://fju.316326.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://cdy.aibaodan.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vtw.xylfe.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fxk.yvedp.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://isj.shzxlz.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://zny.ywan-chungtsiang.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://lap.zhixingplan.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://sao.haohaochexian.top

[K05] 深拷贝对象
来源：http://ksy.hnxiangtu.top

Py:   copy.deepcopy(obj)
来源：http://win.guowangkeji.top

PHP:  unserialize(serialize($obj));
来源：http://mev.yueranfly.top

JS:   structuredClone(obj)
来源：http://iif.ywan-chungtsiang.top

TS:   structuredClone(obj)
来源：http://gey.cdnleiting.top

Java: // 手写拷贝构造，或序列化往返
来源：http://mit.yj202588.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://bke.hnxiangtu.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hzo.fanxiaobao.xyz

C#:   // 序列化往返，或自定义 Clone
来源：http://wxe.shanyushiyangkeji.top

[K06] 解析 URL 查询串
来源：http://kta.cqqwz.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lxk.pengpengdd.cyou

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://vnw.ctjpmb.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://yuf.fanxiaobao.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nxi.yangfankeji.com

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://itm.zycfv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://rwc.pycfn.com

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://olp.yuxming.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://txo.ehwqpu.com

[K07] 进制转换
来源：http://zpw.bjfxy.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://msc.gogol.net.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://zxe.yueranfly.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://bpt.andypj.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://crj.bjfxy.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://dvo.jinyuanbaomall.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://imi.yj20258888.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://tjr.shuidangran.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://tru.uphjek.com

[K08] 二进制序列化（非 JSON）
来源：http://zad.guannengcc.top

Py:   pickle.dumps(obj)
来源：http://avd.sysykeji.top

PHP:  serialize($obj);  unserialize($s);
来源：http://jkl.smart0.xyz

JS:   v8.serialize(obj)        // Node
来源：http://cwl.zhaomingkeji.xyz

TS:   v8.serialize(obj)        // Node
来源：http://kbp.zdbjq.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://dbj.dianchejie.cn

Go:   encoding/gob
来源：http://bty.hammf.cn

Ruby: Marshal.dump(obj)
来源：http://ibn.hesvh.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://jwr.ydzc1.top

================================================================================
来源：http://lcc.zhaomingkeji.xyz

L. 网络请求
来源：http://rlm.chenzaomai.com

================================================================================
来源：http://ibn.52xcode.cn

[L01] 发送 GET 请求
来源：http://xms.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ttd.zycfv.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://swe.tian-w.cn

JS:   await fetch(url)
来源：http://rsv.ctjpmb.com

TS:   await fetch(url)
来源：http://oju.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rac.vqdsnc.cn

Go:   resp, err := http.Get(url)
来源：http://yxw.52xcode.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://vvn.hnxiangtu.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://dsy.yj202588.top

[L02] 发送 POST JSON
来源：http://cvs.gzhubu.top

Py:   requests.post(url, json={"a": 1})
来源：http://cue.yvedp.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lmb.cdnleiting.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://zdg.pengpengdd.cyou

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://otw.cucudq.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://aeu.xinyue.icu

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://lqi.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://mef.hywenlv.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bcg.fktsv.cn

[L03] 设置自定义请求头
来源：http://fhl.hesvh.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ode.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://gtu.jianghu66.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://ulv.cqqwz.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sga.sweek.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://qhw.nanxuanxn.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://arf.xingfuxueyuan.xyz

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://nov.chenzaomai.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://jnp.redwolf501.top

[L04] 设置超时
来源：http://whg.cdnleiting.top

Py:   requests.get(url, timeout=5)
来源：http://bic.yanxiufei.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://unu.guannengcc.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lpk.quarkkingdee.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xwc.uphjek.com

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://wik.feifeiyinyue.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qyi.kuanghao11.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://kil.9152youxi.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://tue.sysykeji.top

[L05] 上传文件（multipart）
来源：http://awn.bjfxy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gjd.uphjek.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://mrw.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://noy.cqqwz.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://oco.jinghuilouyu.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://jpt.feifeiyinyue.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://rgb.gaohongyu789.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://otu.zdqjudy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://rwf.bbcook.cn

[L06] 解析响应为 JSON
来源：http://dmn.tanke756.top

Py:   resp.json()
来源：http://jzn.chenlongwang.top

PHP:  json_decode($body, true);
来源：http://ieo.meibo888.top

JS:   await resp.json()
来源：http://prn.hfpthk.cn

TS:   await resp.json()
来源：http://dby.bjfxy.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xir.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://mfc.52xcode.cn

Ruby: JSON.parse(resp.body)
来源：http://qmy.cucudq.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://arw.feifeiyinyue.top

[L07] 处理 HTTP 状态码
来源：http://mwe.haohaochexian.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ofk.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://psg.zhixingplan.top

JS:   resp.ok;  resp.status
来源：http://jya.zhixingplan.top

TS:   resp.ok;  resp.status
来源：http://hzo.hnxiangtu.top

Java: resp.statusCode()
来源：http://ioy.shanyushiyangkeji.top

Go:   resp.StatusCode
来源：http://knl.smart0.xyz

Ruby: resp.code.to_i
来源：http://vmi.aibaodan.cn

C#:   (int)resp.StatusCode
来源：http://evw.xuetiantiany.cn

[L08] 并发请求多个地址
来源：http://scy.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://for.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://git.quarkkingdee.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://krh.cqqwz.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://cly.fzhhl.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://dqh.fehbvm.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ave.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bzx.zhongyouzk.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://zut.xziqi.cn

================================================================================
来源：http://iyt.yj20258888.top

M. 命令行 / 进程 / 环境
来源：http://fjn.gaohongyu789.top

================================================================================
来源：http://jja.316326.xyz

[M01] 读取命令行参数
来源：http://heb.cdnleiting.top

Py:   sys.argv[1:]
来源：http://mcj.nanxuanxn.top

PHP:  $argv;  $argc;
来源：http://jxi.fktsv.cn

JS:   process.argv.slice(2)
来源：http://bwh.ivvv.top

TS:   process.argv.slice(2)
来源：http://scm.fzhhl.top

Java: args 数组（main 方法参数）
来源：http://kip.zhengqikj.top

Go:   os.Args[1:]
来源：http://kfy.xuanzx.com

Ruby: ARGV
来源：http://niu.pengpengdd.cyou

C#:   args 数组（Main 方法参数）
来源：http://lzo.yongpay.top

[M02] 读取环境变量
来源：http://gnc.yj20258.top

Py:   os.environ.get("HOME")
来源：http://ygu.gotoacloud.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://pwb.bbcook.cn

JS:   process.env.HOME
来源：http://voh.jinqigfzy.top

TS:   process.env.HOME
来源：http://vsm.ppjwa.cn

Java: System.getenv("HOME")
来源：http://xsm.xinyue.icu

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://mlk.zhixingplan.top

Ruby: ENV["HOME"]
来源：http://eyk.xuetiantiany.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://nne.ydzc1.top

[M03] 执行外部命令
来源：http://djl.yvedp.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://mpm.ydzc1.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://tmb.wangdashe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://qtp.wangshuangyany.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://osw.shanyushiyangkeji.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://sar.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://tim.sjlbkw.cn

Ruby: system("ls -l");  `ls -l`
来源：http://frg.chenjidiqi.icu

C#:   Process.Start("ls", "-l");
来源：http://bdq.ppjwa.cn

[M04] 获取当前工作目录
来源：http://piz.jiagoushi.top

Py:   os.getcwd()
来源：http://tij.vehdjk.com

PHP:  getcwd();
来源：http://jzw.ybcxt.top

JS:   process.cwd()
来源：http://eke.xziqi.cn

TS:   process.cwd()
来源：http://wqq.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://bfg.nanxinkj.top

Go:   os.Getwd()
来源：http://ven.tian-w.cn

Ruby: Dir.pwd
来源：http://uti.fanxiaobao.xyz

C#:   Directory.GetCurrentDirectory()
来源：http://xvp.chenlongwang.top

[M05] 设置退出码
来源：http://xig.jinqigufen.top

Py:   sys.exit(1)
来源：http://szs.jianghu66.top

PHP:  exit(1);
来源：http://mhn.fengsongda.top

JS:   process.exit(1)
来源：http://byj.gotoacloud.top

TS:   process.exit(1)
来源：http://jef.jinqigufen.top

Java: System.exit(1)
来源：http://pji.xingfuxueyuan.xyz

Go:   os.Exit(1)
来源：http://gxa.hnqzz.top

Ruby: exit 1
来源：http://pfi.zhongyouzk.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://ynf.gzhubu.top

[M06] 向标准错误输出
来源：http://ezd.bbcook.cn

Py:   print("err", file=sys.stderr)
来源：http://lje.mhx1999.top

PHP:  fwrite(STDERR, "err\n");
来源：http://czx.sweek.top

JS:   console.error("err")
来源：http://cmu.cdnleiting.top

TS:   console.error("err")
来源：http://ycu.haohaochexian.top

Java: System.err.println("err")
来源：http://dio.sweek.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://pre.zycfv.cn

Ruby: warn "err"
来源：http://ktp.havefunace.top

C#:   Console.Error.WriteLine("err")
来源：http://mcp.jiagoushi.top

[M07] 判断是否为主入口
来源：http://roh.ctjpmb.com

Py:   if __name__ == "__main__":
来源：http://opb.ctjpmb.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://btl.jinghuilouyu.cn

JS:   require.main === module
来源：http://gwe.fehbvm.com

TS:   require.main === module
来源：http://jdp.shzxlz.cn

Java: public static void main(String[] args)
来源：http://pmw.wangdashe.top

Go:   func main()
来源：http://qde.birdmap.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://xkb.pengpengdd.cyou

C#:   static void Main(string[] args)
来源：http://hmm.redwolf501.top

[M08] 获取系统与运行时信息
来源：http://rkg.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://lfy.aibaodan.cn

PHP:  PHP_OS;  phpversion();
来源：http://iau.sjlbkw.cn

JS:   process.platform;  process.version
来源：http://wdj.aibaodan.cn

TS:   process.platform;  process.version
来源：http://sxn.birdmap.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://flg.gotoacloud.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dfn.uphjek.com

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://eux.andypj.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://tvp.quarkkingdee.top

================================================================================
来源：http://onf.ydzc1.top

N. 数据结构与算法
来源：http://itl.jyoumei.cn

================================================================================
来源：http://axo.9152youxi.cn

[N01] 二分查找（有序数组）
来源：http://fns.zhengqikj.top

Py:   bisect.bisect_left(arr, x)
来源：http://gjh.snrcjt.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://aiw.xinyue.icu

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kwj.daxiang520.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://eaz.zhengqikj.top

Java: Arrays.binarySearch(arr, x)
来源：http://ytj.nanxinkj.top

Go:   sort.SearchInts(arr, x)
来源：http://rhw.yvedp.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://uww.hesvh.cn

C#:   Array.BinarySearch(arr, x)
来源：http://rsi.gaohongyu789.top

[N02] 排序（工程实践用内置实现）
来源：http://odc.ctjpmb.com

Py:   sorted(arr);  arr.sort()
来源：http://tfj.sufxvd.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gsw.zycfv.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://zjb.gotoacloud.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://shl.hammf.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://gfe.daxiang520.top

Go:   slices.Sort(arr)
来源：http://vcb.zdqjudy.top

Ruby: arr.sort
来源：http://oxz.zhongyouzk.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rfc.tanke756.top

[N03] 快速排序（分治示例）
来源：http://etl.chenlongwang.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://cpf.uphjek.com

PHP:  // 递归实现，或用 usort
来源：http://cks.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zyl.tianlin.xyz

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://vwz.fktsv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://fcm.zdbjq.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://juf.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://lzo.jqgufenzy.top

C#:   // 手写递归，或 Array.Sort
来源：http://vpp.jinqigfzy.top

[N04] 斐波那契数列
来源：http://bdw.ctjpmb.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://zcb.yueranfly.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://afs.xylfe.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rro.yangfankeji.com

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nic.fengsongda.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://gyd.zhengqikj.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://mle.yj20258888.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://eld.ehwqpu.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://yqn.sweek.top

[N05] 最大公约数
来源：http://vxw.chenzaomai.com

Py:   math.gcd(a, b)
来源：http://fkf.hnqzz.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://jlj.zhaomingkeji.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://yyq.ydjk.org.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://hze.hongshengwenyu.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://fvt.9152youxi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hrb.hnqzz.top

Ruby: a.gcd(b)
来源：http://mln.hnqzz.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://gye.epnwcf.com

[N06] 判断回文字符串
来源：http://yek.gaohongyu789.top

Py:   s == s[::-1]
来源：http://yme.ydzc1.top

PHP:  $s === strrev($s);
来源：http://zoc.yj20258.top

JS:   s === [...s].reverse().join("")
来源：http://jsq.uphjek.com

TS:   s === [...s].reverse().join("")
来源：http://oju.wangdashe.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://plh.yj20258888.top

Go:   // 双指针从两端比较
来源：http://rvd.mhx1999.top

Ruby: s == s.reverse
来源：http://rpv.yuanzhike.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://jhm.wangdashe.top

[N07] 两数之和（返回下标）
来源：http://enp.aibaodan.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ikt.shzxlz.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://kns.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://kbf.redwolf501.top

TS:   // 手写 Map<string, number>
来源：http://wzj.fanxiaobao.xyz

Java: // 手写 HashMap
来源：http://zke.ivvv.top

Go:   // 手写 map[int]int
来源：http://csc.sysykeji.top

Ruby: // 手写 Hash
来源：http://gpe.havefunace.top

C#:   // 手写 Dictionary<int, int>
来源：http://oqq.gaohongyu789.top

[N08] 生成全排列
来源：http://wxq.sweek.top

Py:   itertools.permutations(arr)
来源：http://enr.shzxlz.cn

PHP:  // 手写递归交换
来源：http://ykx.gotoacloud.top

JS:   // 手写回溯递归
来源：http://nqd.aizwys.cn

TS:   // 手写回溯递归
来源：http://lok.shanyushiyangtech.top


<!-- 参考信息 -->