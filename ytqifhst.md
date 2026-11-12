代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://jby.zhixingplan.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://igo.shanyushiyangkeji.top

JS:   JSON.stringify(obj)
来源：http://alx.yonumen.top

TS:   JSON.stringify(obj)
来源：http://ked.sufxvd.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://hep.9152youxi.cn

Go:   json.Marshal(obj)
来源：http://kqg.zhijiandao.cn

Ruby: obj.to_json                                     // require "json"
来源：http://xxf.ydzc1.top

C#:   JsonSerializer.Serialize(obj)
来源：http://hcf.sufxvd.cn

[K02] JSON 字符串转对象
来源：http://swh.jinghuilouyu.cn

Py:   json.loads(s)
来源：http://swh.fehbvm.com

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://xtf.tianlin.xyz

JS:   JSON.parse(s)
来源：http://mpm.shanyushiyangkeji.top

TS:   JSON.parse(s)
来源：http://jba.yongpay.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://zjd.guowangkeji.top

Go:   json.Unmarshal(data, &v)
来源：http://nly.pengpengdd.cyou

Ruby: JSON.parse(s)
来源：http://cqb.316326.xyz

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://lha.nanxuanxn.top

[K03] JSON 美化输出（带缩进）
来源：http://yxa.tianlin.xyz

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xtj.yueranfly.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://trj.andypj.xyz

JS:   JSON.stringify(obj, null, 2)
来源：http://pxa.sjlbkw.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://eci.gogol.net.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://aij.jinyuanbaomall.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://rhv.zdqjudy.top

Ruby: JSON.pretty_generate(obj)
来源：http://eus.yvedp.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mqd.jianghu66.top

[K04] 读取 JSON 文件
来源：http://son.52xcode.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://jxz.nanxinkj.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://zah.hongshengwenyu.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jcy.hongshengwenyu.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vnv.tian-w.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://sxf.feifeiyinyue.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://xbu.fengsongda.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://feo.mhx1999.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vgu.vehdjk.com

[K05] 深拷贝对象
来源：http://lwc.ehwqpu.com

Py:   copy.deepcopy(obj)
来源：http://okc.sufxvd.cn

PHP:  unserialize(serialize($obj));
来源：http://gjf.haohaochexian.top

JS:   structuredClone(obj)
来源：http://udd.zhongyouzk.top

TS:   structuredClone(obj)
来源：http://lke.jinyuanbaomall.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://svw.gzhubu.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://jsz.cashguo.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://lng.gogol.net.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://mhm.yongpay.top

[K06] 解析 URL 查询串
来源：http://rqc.fehbvm.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://spq.zhongyouzk.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://zmc.gaohongyu789.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://xxi.jyoumei.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://cte.fanxiaobao.xyz

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://wyt.pycfn.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://pcj.shzxlz.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://vlb.guannengcc.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://vrt.ywan-chungtsiang.top

[K07] 进制转换
来源：http://vew.cashguo.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hjh.ydjk.org.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://ypx.zdbjq.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://yib.gogol.net.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://oua.birdmap.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://vmj.zhiwuduotai.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ngy.shanyushiyangtech.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://crz.aibaodan.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ude.birdmap.top

[K08] 二进制序列化（非 JSON）
来源：http://pcj.52xcode.cn

Py:   pickle.dumps(obj)
来源：http://trm.52xcode.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://yqq.nwbrower.top

JS:   v8.serialize(obj)        // Node
来源：http://kmp.hesvh.cn

TS:   v8.serialize(obj)        // Node
来源：http://gac.pycfn.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://kqy.shanyushiyangtech.top

Go:   encoding/gob
来源：http://hsp.tanke756.top

Ruby: Marshal.dump(obj)
来源：http://tbz.gzhubu.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://luy.epnwcf.com

================================================================================
来源：http://dsk.yfazqb.com

L. 网络请求
来源：http://ypx.xuetiantiany.cn

================================================================================
来源：http://fpi.guowangkeji.top

[L01] 发送 GET 请求
来源：http://qyh.svipenyu.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://vik.ydzc1.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://lmr.xziqi.cn

JS:   await fetch(url)
来源：http://juy.yj20258.top

TS:   await fetch(url)
来源：http://kgg.yj20258888.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://ytz.cucudq.cn

Go:   resp, err := http.Get(url)
来源：http://ycx.ybcxt.top

Ruby: Net::HTTP.get(URI(url))
来源：http://ipf.fengsongda.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://vgd.ybcxt.top

[L02] 发送 POST JSON
来源：http://tiq.xuetiantiany.cn

Py:   requests.post(url, json={"a": 1})
来源：http://rhy.shanyushiyangtech.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://lsp.uphjek.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fpu.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://eyh.nwbrower.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ppl.xylfe.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://omk.yj20258.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://kyd.yj20258888.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://rvh.zdbjq.cn

[L03] 设置自定义请求头
来源：http://pfr.quarkkingdee.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://gyk.hnqzz.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://xdv.xuanzx.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hgc.redwolf501.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://yvp.xinyue.icu

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hnj.quarkkingdee.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xbr.hongshengwenyu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://rwz.svipenyu.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://wve.chenlongwang.top

[L04] 设置超时
来源：http://lwq.aizwys.cn

Py:   requests.get(url, timeout=5)
来源：http://wyi.nwbrower.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tbc.gaohongyu789.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jrq.zhoulong.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vbi.xylfe.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kyy.9152youxi.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://hij.sjlbkw.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dlq.hywenlv.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://snv.nanxinkj.top

[L05] 上传文件（multipart）
来源：http://eoa.gogol.net.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://nko.yuanzhike.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ngj.chenzaomai.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://nbk.jqgfzy.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://aku.kuanghao11.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://vxp.gotoacloud.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://eps.chenjidiqi.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://enk.jinghuilouyu.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://zea.zycfv.cn

[L06] 解析响应为 JSON
来源：http://hgo.zhixingplan.top

Py:   resp.json()
来源：http://pda.jianghu66.top

PHP:  json_decode($body, true);
来源：http://soc.guowangkeji.top

JS:   await resp.json()
来源：http://bwd.wangshuangyany.cn

TS:   await resp.json()
来源：http://bhb.zhiwuduotai.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://lbt.meibo888.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://uer.fengsongda.top

Ruby: JSON.parse(resp.body)
来源：http://kga.cashguo.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://ptl.xylfe.cn

[L07] 处理 HTTP 状态码
来源：http://toz.daxiang520.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://oux.9152youxi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://gbs.bjfxy.top

JS:   resp.ok;  resp.status
来源：http://gdn.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://cnf.316326.xyz

Java: resp.statusCode()
来源：http://uja.zdqjudy.top

Go:   resp.StatusCode
来源：http://olc.zhongyouzk.top

Ruby: resp.code.to_i
来源：http://iuj.hongshengwenyu.top

C#:   (int)resp.StatusCode
来源：http://kqp.svipenyu.cn

[L08] 并发请求多个地址
来源：http://xhw.sjlbkw.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://rha.redwolf501.top

PHP:  curl_multi_init() 系列
来源：http://fhi.bbcook.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://oqm.jinqigfzy.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://axo.cqqwz.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ini.shanyushiyangtech.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ceh.yongpay.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://qey.cheryme.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://tug.xziqi.cn

================================================================================
来源：http://ycm.jiagoushi.top

M. 命令行 / 进程 / 环境
来源：http://tho.jiagoushi.top

================================================================================
来源：http://ikr.andypj.xyz

[M01] 读取命令行参数
来源：http://rcf.yonumen.top

Py:   sys.argv[1:]
来源：http://zoy.ydjk.org.cn

PHP:  $argv;  $argc;
来源：http://pih.snrcjt.cn

JS:   process.argv.slice(2)
来源：http://vsm.jianghu66.top

TS:   process.argv.slice(2)
来源：http://wgw.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://rzg.sufxvd.cn

Go:   os.Args[1:]
来源：http://ajn.hysaishi.cn

Ruby: ARGV
来源：http://tji.sjlbkw.cn

C#:   args 数组（Main 方法参数）
来源：http://acj.jqgfzy.top

[M02] 读取环境变量
来源：http://hyr.52xcode.cn

Py:   os.environ.get("HOME")
来源：http://wdt.jinyuanbaomall.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://jby.meibo888.top

JS:   process.env.HOME
来源：http://cgx.cashguo.top

TS:   process.env.HOME
来源：http://lni.316326.xyz

Java: System.getenv("HOME")
来源：http://nne.316326.xyz

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://bai.daria6918.cn

Ruby: ENV["HOME"]
来源：http://ekt.fzhhl.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://dul.sweek.top

[M03] 执行外部命令
来源：http://ekl.zhaomingkeji.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yvb.jinghuilouyu.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://kge.fktsv.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xwh.yonumen.top

TS:   child_process.execSync("ls -l").toString()
来源：http://ave.hysaishi.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://huq.yangfankeji.com

Go:   exec.Command("ls", "-l").Output()
来源：http://bhd.tarul.cn

Ruby: system("ls -l");  `ls -l`
来源：http://cpp.ehwqpu.com

C#:   Process.Start("ls", "-l");
来源：http://nel.cucudq.cn

[M04] 获取当前工作目录
来源：http://tcw.zhongyouzk.top

Py:   os.getcwd()
来源：http://bbi.yfazqb.com

PHP:  getcwd();
来源：http://rip.shanyushiyangkeji.top

JS:   process.cwd()
来源：http://uay.shuidangran.top

TS:   process.cwd()
来源：http://mwy.shanyushiyangkeji.top

Java: Path.of("").toAbsolutePath()
来源：http://ihs.jiagoushi.top

Go:   os.Getwd()
来源：http://alw.ctjpmb.com

Ruby: Dir.pwd
来源：http://whr.0kj1m.cn

C#:   Directory.GetCurrentDirectory()
来源：http://sxu.sufxvd.cn

[M05] 设置退出码
来源：http://fsm.gotoacloud.top

Py:   sys.exit(1)
来源：http://emo.yanxiufei.cn

PHP:  exit(1);
来源：http://kld.ybcxt.top

JS:   process.exit(1)
来源：http://lyq.pycfn.com

TS:   process.exit(1)
来源：http://bnb.hfpthk.cn

Java: System.exit(1)
来源：http://xai.zhengqikj.top

Go:   os.Exit(1)
来源：http://eec.ivvv.top

Ruby: exit 1
来源：http://qmh.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vxr.cheryme.top

[M06] 向标准错误输出
来源：http://mcl.nwbrower.top

Py:   print("err", file=sys.stderr)
来源：http://vnu.havefunace.top

PHP:  fwrite(STDERR, "err\n");
来源：http://kug.jinyuanbaomall.cn

JS:   console.error("err")
来源：http://txt.ehwqpu.com

TS:   console.error("err")
来源：http://cxl.zhiwuduotai.top

Java: System.err.println("err")
来源：http://cbt.hnqzz.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hrq.yanxiufei.cn

Ruby: warn "err"
来源：http://myi.sysykeji.top

C#:   Console.Error.WriteLine("err")
来源：http://gdu.jianghu66.top

[M07] 判断是否为主入口
来源：http://gmj.tianlin.xyz

Py:   if __name__ == "__main__":
来源：http://boh.yuanzhike.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gmq.hnqzz.top

JS:   require.main === module
来源：http://zkd.fzhhl.top

TS:   require.main === module
来源：http://axj.svipenyu.cn

Java: public static void main(String[] args)
来源：http://qkf.jiagoushi.top

Go:   func main()
来源：http://lqc.ctjpmb.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://eoe.ywan-chungtsiang.top

C#:   static void Main(string[] args)
来源：http://nsn.svipenyu.cn

[M08] 获取系统与运行时信息
来源：http://kuw.guowangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://ilj.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://idx.hongshengwenyu.top

JS:   process.platform;  process.version
来源：http://vmd.daxiang520.top

TS:   process.platform;  process.version
来源：http://yzk.yj20258888.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://hbl.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://xww.tarul.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rdv.zhaomingkeji.xyz

C#:   Environment.OSVersion;  Environment.Version
来源：http://gvg.gotoacloud.top

================================================================================
来源：http://jke.zhiwuduotai.top

N. 数据结构与算法
来源：http://sud.nwbrower.top

================================================================================
来源：http://lxp.jianghu66.top

[N01] 二分查找（有序数组）
来源：http://sdc.chenjidiqi.icu

Py:   bisect.bisect_left(arr, x)
来源：http://lyk.nwbrower.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://axz.ybcxt.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://zqq.tarul.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nnf.aibaodan.cn

Java: Arrays.binarySearch(arr, x)
来源：http://tvq.ivvv.top

Go:   sort.SearchInts(arr, x)
来源：http://iwp.xinyue.icu

Ruby: arr.bsearch { |e| e >= x }
来源：http://plr.jlsjyb.cn

C#:   Array.BinarySearch(arr, x)
来源：http://kau.hywenlv.cn

[N02] 排序（工程实践用内置实现）
来源：http://piw.shanyushiyangkeji.top

Py:   sorted(arr);  arr.sort()
来源：http://brm.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://oef.tian-w.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://kkc.yj20258888.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://gli.fzhhl.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ufz.gogol.net.cn

Go:   slices.Sort(arr)
来源：http://njg.hfpthk.cn

Ruby: arr.sort
来源：http://cwo.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://rcg.kuanghao11.cn

[N03] 快速排序（分治示例）
来源：http://xxi.xuanzx.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://grt.9152youxi.cn

PHP:  // 递归实现，或用 usort
来源：http://yla.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://uqk.ydzc1.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://fgq.nanxinkj.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://zhn.snrcjt.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://fry.zdqjudy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://dgp.jinyuanbaomall.cn

C#:   // 手写递归，或 Array.Sort
来源：http://pal.nanxuanxn.top

[N04] 斐波那契数列
来源：http://ybk.zhijiandao.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://sdh.shuidangran.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kvt.hnqzz.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://csy.hywenlv.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eqv.gaohongyu789.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://ulg.ydjk.org.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lst.0kj1m.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://fov.zhijiandao.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kfh.yj20258888.top

[N05] 最大公约数
来源：http://www.nwbrower.top

Py:   math.gcd(a, b)
来源：http://ubt.aizwys.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tyo.xylfe.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jot.epnwcf.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rok.hfpthk.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://yqy.tarul.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://bri.yj20258888.top

Ruby: a.gcd(b)
来源：http://ywq.hammf.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://dln.snrcjt.cn

[N06] 判断回文字符串
来源：http://tfr.dashuyun.cn

Py:   s == s[::-1]
来源：http://cyf.jlsjyb.cn

PHP:  $s === strrev($s);
来源：http://gls.fengsongda.top

JS:   s === [...s].reverse().join("")
来源：http://veh.sufxvd.cn

TS:   s === [...s].reverse().join("")
来源：http://oxp.zhijiandao.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bnt.pycfn.com

Go:   // 双指针从两端比较
来源：http://kqk.ybcxt.top

Ruby: s == s.reverse
来源：http://ygw.gzhubu.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://bkb.nwbrower.top

[N07] 两数之和（返回下标）
来源：http://pqe.haohaochexian.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://yub.chenjidiqi.icu

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ozo.yangfankeji.com

JS:   // 手写 Map：map.set(v, i)
来源：http://mpi.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://vzm.uphjek.com

Java: // 手写 HashMap
来源：http://gop.yueranfly.top

Go:   // 手写 map[int]int
来源：http://lem.yuxming.cn

Ruby: // 手写 Hash
来源：http://rxe.zycfv.cn

C#:   // 手写 Dictionary<int, int>
来源：http://aoi.wangshuangyany.cn

[N08] 生成全排列
来源：http://woq.pengpengdd.cyou

Py:   itertools.permutations(arr)
来源：http://ntl.fzhhl.top

PHP:  // 手写递归交换
来源：http://bmo.daria6918.cn

JS:   // 手写回溯递归
来源：http://nob.hongshengwenyu.top

TS:   // 手写回溯递归
来源：http://wzb.shanyushiyangkeji.top

Java: // 手写回溯递归
来源：http://wri.yangfankeji.com

Go:   // 手写回溯递归
来源：http://vji.ydzc1.top

Ruby: arr.permutation.to_a
来源：http://dor.birdmap.top

C#:   // 手写回溯递归
来源：http://kzr.jinqigufen.top

[N09] 栈与队列
来源：http://vwq.dianchejie.cn

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://tbn.sufxvd.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://utp.sweek.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://uet.yuanzhike.top


<!-- 参考信息 -->