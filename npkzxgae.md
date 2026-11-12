代发 wailian999

================================================================================
来源：http://iei.aibaodan.cn

K. JSON 与序列化
来源：http://ase.chenzaomai.com

================================================================================
来源：http://gup.ivvv.top

[K01] 对象转 JSON 字符串
来源：http://vim.nanxinkj.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://smj.cdnleiting.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://fps.chenlongwang.top

JS:   JSON.stringify(obj)
来源：http://vtq.shuidangran.top

TS:   JSON.stringify(obj)
来源：http://had.tian-w.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://dbp.cdnleiting.top

Go:   json.Marshal(obj)
来源：http://beg.uphjek.com

Ruby: obj.to_json                                     // require "json"
来源：http://jyj.ppjwa.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://cuw.jinqigfzy.top

[K02] JSON 字符串转对象
来源：http://iro.ydzc1.top

Py:   json.loads(s)
来源：http://hro.jyoumei.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://cxn.jlsjyb.cn

JS:   JSON.parse(s)
来源：http://gnw.yongpay.top

TS:   JSON.parse(s)
来源：http://jex.redwolf501.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://pyx.ydjk.org.cn

Go:   json.Unmarshal(data, &v)
来源：http://bxn.cdnleiting.top

Ruby: JSON.parse(s)
来源：http://xno.zhiwuduotai.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://odd.cashguo.top

[K03] JSON 美化输出（带缩进）
来源：http://xhm.xziqi.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://cql.meibo888.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://gru.hnqzz.top

JS:   JSON.stringify(obj, null, 2)
来源：http://hkn.vqdsnc.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xzj.fktsv.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://pqq.xinyue.icu

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nvq.cdnleiting.top

Ruby: JSON.pretty_generate(obj)
来源：http://qbq.zhengqikj.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://tnw.yvedp.cn

[K04] 读取 JSON 文件
来源：http://sau.jinqigufen.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tid.sysykeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://azx.hnqzz.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://xop.yuanzhike.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://rjk.xziqi.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://dqu.zdbjq.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ejq.hnxiangtu.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://jel.zycfv.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vvp.aibaodan.cn

[K05] 深拷贝对象
来源：http://xkb.ppjwa.cn

Py:   copy.deepcopy(obj)
来源：http://igc.wangdashe.top

PHP:  unserialize(serialize($obj));
来源：http://rbp.gaohongyu789.top

JS:   structuredClone(obj)
来源：http://fnm.sxryk.cn

TS:   structuredClone(obj)
来源：http://dpp.xinyue.icu

Java: // 手写拷贝构造，或序列化往返
来源：http://xnk.tarul.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://qdv.hcnkem.com

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://nce.birdmap.top

C#:   // 序列化往返，或自定义 Clone
来源：http://zwn.iojbl.cn

[K06] 解析 URL 查询串
来源：http://bwk.sysykeji.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://yil.snrcjt.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://boy.nwbrower.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://okt.zhaomingkeji.xyz

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://gcb.9152youxi.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://cki.fktsv.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://iea.zhiwuduotai.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ygl.fzhhl.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pei.ydzc1.top

[K07] 进制转换
来源：http://wkk.yonumen.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://hrr.wangshuangyany.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://lhn.cqqwz.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vdq.yanxiufei.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://qty.ppjwa.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://tga.hysaishi.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://uxf.ctjpmb.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://poi.zhengqikj.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://duj.yuanzhike.top

[K08] 二进制序列化（非 JSON）
来源：http://rbd.snrcjt.cn

Py:   pickle.dumps(obj)
来源：http://lwu.xziqi.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://zvn.hfpthk.cn

JS:   v8.serialize(obj)        // Node
来源：http://pvp.jianghu66.top

TS:   v8.serialize(obj)        // Node
来源：http://odn.ehwqpu.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://aei.yangfankeji.com

Go:   encoding/gob
来源：http://dxr.tian-w.cn

Ruby: Marshal.dump(obj)
来源：http://cie.shanyushiyangkeji.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://tba.birdmap.top

================================================================================
来源：http://qho.jqgfzy.top

L. 网络请求
来源：http://uql.havefunace.top

================================================================================
来源：http://wae.ehwqpu.com

[L01] 发送 GET 请求
来源：http://bgq.birdmap.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ork.uphjek.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://fhd.shuidangran.top

JS:   await fetch(url)
来源：http://agf.jqgfzy.top

TS:   await fetch(url)
来源：http://gmt.sxryk.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rkm.hysaishi.cn

Go:   resp, err := http.Get(url)
来源：http://akb.nanxuanxn.top

Ruby: Net::HTTP.get(URI(url))
来源：http://onf.hnqzz.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://wsf.ybcxt.top

[L02] 发送 POST JSON
来源：http://frf.fanxiaobao.xyz

Py:   requests.post(url, json={"a": 1})
来源：http://fjd.aizwys.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://jkq.yueranfly.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://uqy.yongpay.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jql.sufxvd.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://kpr.jyoumei.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://yvu.hywenlv.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://vnc.dashuyun.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://gwf.wangdashe.top

[L03] 设置自定义请求头
来源：http://hel.ivvv.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ald.zycfv.cn

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://zxs.jyoumei.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sfj.jinqigufen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zob.c1oappe.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://gho.daxiang520.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://hgm.zdbjq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://wjs.jyoumei.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hqh.sxryk.cn

[L04] 设置超时
来源：http://ukz.zycfv.cn

Py:   requests.get(url, timeout=5)
来源：http://uyc.hcnkem.com

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zaw.fehbvm.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://sqj.fzhhl.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://lcq.iojbl.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cuc.jqgfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://vxn.svipenyu.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://tkv.shanyushiyangtech.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://iyj.jqgufenzy.top

[L05] 上传文件（multipart）
来源：http://jth.cqqwz.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://yyp.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://cdz.yj202588.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://tlr.svipenyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://jze.dashuyun.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://yur.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://onw.shanyushiyangtech.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mvd.sjlbkw.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ava.guowangkeji.top

[L06] 解析响应为 JSON
来源：http://myj.nanxuanxn.top

Py:   resp.json()
来源：http://zox.jiagoushi.top

PHP:  json_decode($body, true);
来源：http://oxu.quarkkingdee.top

JS:   await resp.json()
来源：http://zoj.cqqwz.cn

TS:   await resp.json()
来源：http://fvz.andypj.xyz

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cov.hcnkem.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://kco.jlsjyb.cn

Ruby: JSON.parse(resp.body)
来源：http://rgl.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kuu.cucudq.cn

[L07] 处理 HTTP 状态码
来源：http://nlr.c1oappe.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zfo.daxiang520.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sct.jqgfzy.top

JS:   resp.ok;  resp.status
来源：http://kcy.sxryk.cn

TS:   resp.ok;  resp.status
来源：http://hkw.xingfuxueyuan.xyz

Java: resp.statusCode()
来源：http://rrh.pengpengdd.cyou

Go:   resp.StatusCode
来源：http://swb.chenjidiqi.icu

Ruby: resp.code.to_i
来源：http://fwv.cheryme.top

C#:   (int)resp.StatusCode
来源：http://nyh.52xcode.cn

[L08] 并发请求多个地址
来源：http://wzv.gzhubu.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://kzg.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://dom.316326.xyz

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://umn.ctjpmb.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://uno.pycfn.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://xlt.cucudq.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://byy.nanxuanxn.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://emi.xuetiantiany.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://ukx.ppjwa.cn

================================================================================
来源：http://ecz.fktsv.cn

M. 命令行 / 进程 / 环境
来源：http://atu.hongshengwenyu.top

================================================================================
来源：http://rcv.wangshuangyany.cn

[M01] 读取命令行参数
来源：http://ahe.bjfxy.top

Py:   sys.argv[1:]
来源：http://tjw.xuanzx.com

PHP:  $argv;  $argc;
来源：http://igm.zhixingplan.top

JS:   process.argv.slice(2)
来源：http://pkm.smart0.xyz

TS:   process.argv.slice(2)
来源：http://xjc.nanxuanxn.top

Java: args 数组（main 方法参数）
来源：http://rvt.gaohongyu789.top

Go:   os.Args[1:]
来源：http://ffh.daxiang520.top

Ruby: ARGV
来源：http://yld.daria6918.cn

C#:   args 数组（Main 方法参数）
来源：http://znh.zhengqikj.top

[M02] 读取环境变量
来源：http://yhc.nwbrower.top

Py:   os.environ.get("HOME")
来源：http://lhg.shanyushiyangtech.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qfi.jlsjyb.cn

JS:   process.env.HOME
来源：http://aox.tian-w.cn

TS:   process.env.HOME
来源：http://upy.yvedp.cn

Java: System.getenv("HOME")
来源：http://pvq.xylfe.cn

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wyx.yanxiufei.cn

Ruby: ENV["HOME"]
来源：http://dul.kuanghao11.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ufl.ctjpmb.com

[M03] 执行外部命令
来源：http://dzk.zdqjudy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://yhv.cqqwz.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wgx.jinghuilouyu.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://xkj.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://rtf.yj20258888.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://dnr.dashuyun.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://ojr.haohaochexian.top

Ruby: system("ls -l");  `ls -l`
来源：http://trp.yangfankeji.com

C#:   Process.Start("ls", "-l");
来源：http://czs.sweek.top

[M04] 获取当前工作目录
来源：http://uwi.aibaodan.cn

Py:   os.getcwd()
来源：http://xgx.jqgufenzy.top

PHP:  getcwd();
来源：http://osp.yj20258.top

JS:   process.cwd()
来源：http://yid.yfazqb.com

TS:   process.cwd()
来源：http://sfz.fengsongda.top

Java: Path.of("").toAbsolutePath()
来源：http://bng.dianchejie.cn

Go:   os.Getwd()
来源：http://jpw.yj202588.top

Ruby: Dir.pwd
来源：http://rev.shzxlz.cn

C#:   Directory.GetCurrentDirectory()
来源：http://blm.xinyue.icu

[M05] 设置退出码
来源：http://snf.wangshuangyany.cn

Py:   sys.exit(1)
来源：http://evm.zhixingplan.top

PHP:  exit(1);
来源：http://icq.sufxvd.cn

JS:   process.exit(1)
来源：http://jds.dianchejie.cn

TS:   process.exit(1)
来源：http://tuv.dianchejie.cn

Java: System.exit(1)
来源：http://hkl.zhijiandao.cn

Go:   os.Exit(1)
来源：http://bti.nanxuanxn.top

Ruby: exit 1
来源：http://scx.cdnleiting.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://mtq.dianchejie.cn

[M06] 向标准错误输出
来源：http://deq.iojbl.cn

Py:   print("err", file=sys.stderr)
来源：http://pzy.birdmap.top

PHP:  fwrite(STDERR, "err\n");
来源：http://yfx.9152youxi.cn

JS:   console.error("err")
来源：http://mbc.vqdsnc.cn

TS:   console.error("err")
来源：http://bwn.hfpthk.cn

Java: System.err.println("err")
来源：http://non.daria6918.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dwp.jqgufenzy.top

Ruby: warn "err"
来源：http://spl.sweek.top

C#:   Console.Error.WriteLine("err")
来源：http://wxu.sufxvd.cn

[M07] 判断是否为主入口
来源：http://ohq.hnxiangtu.top

Py:   if __name__ == "__main__":
来源：http://yal.guowangkeji.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://gnv.yuxming.cn

JS:   require.main === module
来源：http://wzq.andypj.xyz

TS:   require.main === module
来源：http://hyx.0kj1m.cn

Java: public static void main(String[] args)
来源：http://xdv.svipenyu.cn

Go:   func main()
来源：http://psh.pycfn.com

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ppa.redwolf501.top

C#:   static void Main(string[] args)
来源：http://eoc.hongshengwenyu.top

[M08] 获取系统与运行时信息
来源：http://pek.nanxinkj.top

Py:   platform.system();  platform.python_version()
来源：http://bhy.yanxiufei.cn

PHP:  PHP_OS;  phpversion();
来源：http://gmn.hnxiangtu.top

JS:   process.platform;  process.version
来源：http://pru.zhiwuduotai.top

TS:   process.platform;  process.version
来源：http://ise.xuetiantiany.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://ygb.zdbjq.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://nxh.havefunace.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://fkl.dashuyun.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://jqb.cashguo.top

================================================================================
来源：http://kpo.c1oappe.top

N. 数据结构与算法
来源：http://dxn.daria6918.cn

================================================================================
来源：http://lco.xylfe.cn

[N01] 二分查找（有序数组）
来源：http://iur.bjfxy.top

Py:   bisect.bisect_left(arr, x)
来源：http://tsi.snrcjt.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://oeh.zhengqikj.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://pdh.hnqzz.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://qox.shanyushiyangtech.top

Java: Arrays.binarySearch(arr, x)
来源：http://qpm.pycfn.com

Go:   sort.SearchInts(arr, x)
来源：http://wnm.ehwqpu.com

Ruby: arr.bsearch { |e| e >= x }
来源：http://xpt.pengpengdd.cyou

C#:   Array.BinarySearch(arr, x)
来源：http://xez.zhiwuduotai.top

[N02] 排序（工程实践用内置实现）
来源：http://exq.cheryme.top

Py:   sorted(arr);  arr.sort()
来源：http://udw.ybcxt.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ogv.sysykeji.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://hqe.0kj1m.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://ihd.jlsjyb.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://dyq.tian-w.cn

Go:   slices.Sort(arr)
来源：http://txn.yuxming.cn

Ruby: arr.sort
来源：http://wys.xziqi.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://cvd.shuidangran.top

[N03] 快速排序（分治示例）
来源：http://ytz.yonumen.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://fzp.snrcjt.cn

PHP:  // 递归实现，或用 usort
来源：http://qsg.fzhhl.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nub.gotoacloud.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cpw.zhiwuduotai.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://nqf.yueranfly.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ysw.52xcode.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://kit.meibo888.top

C#:   // 手写递归，或 Array.Sort
来源：http://del.hammf.cn

[N04] 斐波那契数列
来源：http://keu.yueranfly.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://qyd.havefunace.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://kkl.hywenlv.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://bsc.xingfuxueyuan.xyz

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://gkg.ybcxt.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://cdu.yueranfly.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://gdf.ywan-chungtsiang.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://iao.tarul.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://exd.hnxiangtu.top

[N05] 最大公约数
来源：http://gbi.svipenyu.cn

Py:   math.gcd(a, b)
来源：http://hbi.jqgufenzy.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://szf.yonumen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://uaz.svipenyu.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://qqo.cheryme.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://omn.zhongyouzk.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://mzu.uphjek.com

Ruby: a.gcd(b)
来源：http://vzh.fehbvm.com

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tfi.sysykeji.top

[N06] 判断回文字符串
来源：http://gqa.yonumen.top

Py:   s == s[::-1]
来源：http://wgh.vehdjk.com

PHP:  $s === strrev($s);
来源：http://mjt.wangdashe.top

JS:   s === [...s].reverse().join("")
来源：http://wap.iojbl.cn

TS:   s === [...s].reverse().join("")
来源：http://iyu.vehdjk.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yqm.zhoulong.xyz

Go:   // 双指针从两端比较
来源：http://wuc.nanxinkj.top

Ruby: s == s.reverse
来源：http://rec.cqqwz.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://cso.redwolf501.top

[N07] 两数之和（返回下标）
来源：http://dzs.ivvv.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://soi.ehwqpu.com

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://soc.sjlbkw.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://juk.jinqigfzy.top

TS:   // 手写 Map<string, number>
来源：http://ahk.cdnleiting.top

Java: // 手写 HashMap
来源：http://aog.fengsongda.top

Go:   // 手写 map[int]int
来源：http://jij.pycfn.com

Ruby: // 手写 Hash
来源：http://gax.shanyushiyangtech.top

C#:   // 手写 Dictionary<int, int>
来源：http://ppa.xylfe.cn

[N08] 生成全排列
来源：http://rhu.gotoacloud.top

Py:   itertools.permutations(arr)
来源：http://wgm.yj202588.top

PHP:  // 手写递归交换
来源：http://yks.dashuyun.cn

JS:   // 手写回溯递归
来源：http://siz.xuanzx.com

TS:   // 手写回溯递归
来源：http://zds.ehwqpu.com

Java: // 手写回溯递归
来源：http://kcd.ppjwa.cn

Go:   // 手写回溯递归
来源：http://enb.redwolf501.top

Ruby: arr.permutation.to_a
来源：http://nxx.jinqigufen.top

C#:   // 手写回溯递归
来源：http://cox.cucudq.cn


<!-- 参考信息 -->