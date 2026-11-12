代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://dux.dashuyun.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://nuc.yj20258.top

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://pvi.ydjk.org.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xdh.fktsv.cn

================================================================================
来源：http://ksu.fzhhl.top

K. JSON 与序列化
来源：http://djx.tianlin.xyz

================================================================================
来源：http://xin.andypj.xyz

[K01] 对象转 JSON 字符串
来源：http://cdt.hongshengwenyu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://xmq.hnqzz.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://hia.gaohongyu789.top

JS:   JSON.stringify(obj)
来源：http://pag.aibaodan.cn

TS:   JSON.stringify(obj)
来源：http://spe.cqqwz.cn

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://scf.shzxlz.cn

Go:   json.Marshal(obj)
来源：http://xxj.ehwqpu.com

Ruby: obj.to_json                                     // require "json"
来源：http://syu.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://otw.chenlongwang.top

[K02] JSON 字符串转对象
来源：http://owx.shzxlz.cn

Py:   json.loads(s)
来源：http://exg.zhongyouzk.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://lfv.jqgufenzy.top

JS:   JSON.parse(s)
来源：http://cjr.xziqi.cn

TS:   JSON.parse(s)
来源：http://hau.zhijiandao.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://udd.shangyingyoupin.top

Go:   json.Unmarshal(data, &v)
来源：http://fgy.yongpay.top

Ruby: JSON.parse(s)
来源：http://wub.daxiang520.top

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://quv.guowangkeji.top

[K03] JSON 美化输出（带缩进）
来源：http://pgb.ivvv.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://yey.pengpengdd.cyou

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ksi.yfazqb.com

JS:   JSON.stringify(obj, null, 2)
来源：http://kze.jinqigfzy.top

TS:   JSON.stringify(obj, null, 2)
来源：http://isn.epnwcf.com

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://rbi.yfazqb.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ldh.zhoulong.xyz

Ruby: JSON.pretty_generate(obj)
来源：http://uwu.dianchejie.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://ciq.jianghu66.top

[K04] 读取 JSON 文件
来源：http://bsq.jinyuanbaomall.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qwh.feifeiyinyue.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rav.xuetiantiany.cn

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://cut.zhongyouzk.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://fzs.shzxlz.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://gfh.hcnkem.com

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://cbb.jiagoushi.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://hxu.cheryme.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vdr.hongshengwenyu.top

[K05] 深拷贝对象
来源：http://nhi.hnqzz.top

Py:   copy.deepcopy(obj)
来源：http://ffb.zdqjudy.top

PHP:  unserialize(serialize($obj));
来源：http://jck.0kj1m.cn

JS:   structuredClone(obj)
来源：http://wav.shuidangran.top

TS:   structuredClone(obj)
来源：http://ilh.hammf.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://nkh.gotoacloud.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://shn.yj20258888.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hmh.xylfe.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://dpn.snrcjt.cn

[K06] 解析 URL 查询串
来源：http://wsc.sjlbkw.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jmo.hnxiangtu.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://sda.epnwcf.com

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://qqu.zhixingplan.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://evw.wangshuangyany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://kqd.andypj.xyz

Go:   url.ParseQuery("a=1&b=2")
来源：http://kwy.sjlbkw.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://gsh.shuidangran.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://xnz.tarul.cn

[K07] 进制转换
来源：http://exj.zhongyouzk.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://qkv.tarul.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://yti.dianchejie.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://vqo.zhongyouzk.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pvx.zhaomingkeji.xyz

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wxr.snrcjt.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://lfw.uphjek.com

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nwu.dashuyun.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ftg.zycfv.cn

[K08] 二进制序列化（非 JSON）
来源：http://jyr.dianchejie.cn

Py:   pickle.dumps(obj)
来源：http://qih.gzhubu.top

PHP:  serialize($obj);  unserialize($s);
来源：http://yhu.zhixingplan.top

JS:   v8.serialize(obj)        // Node
来源：http://vbd.gaohongyu789.top

TS:   v8.serialize(obj)        // Node
来源：http://qjs.chenjidiqi.icu

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://eqo.cashguo.top

Go:   encoding/gob
来源：http://bnf.xuanzx.com

Ruby: Marshal.dump(obj)
来源：http://moo.nwbrower.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://cas.ivvv.top

================================================================================
来源：http://rpr.yuxming.cn

L. 网络请求
来源：http://ggy.shuidangran.top

================================================================================
来源：http://has.gzhubu.top

[L01] 发送 GET 请求
来源：http://xtl.fzhhl.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://tqg.yueranfly.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://kvp.ehwqpu.com

JS:   await fetch(url)
来源：http://frc.fanxiaobao.xyz

TS:   await fetch(url)
来源：http://pti.fengsongda.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://hlp.xuanzx.com

Go:   resp, err := http.Get(url)
来源：http://bif.yj20258888.top

Ruby: Net::HTTP.get(URI(url))
来源：http://fhx.ydzc1.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://xov.ppjwa.cn

[L02] 发送 POST JSON
来源：http://nnc.shanyushiyangtech.top

Py:   requests.post(url, json={"a": 1})
来源：http://ipa.wangdashe.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://tgu.shangyingyoupin.top

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qlw.hcnkem.com

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://odq.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hpz.pycfn.com

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wuy.smart0.xyz

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://xxi.vehdjk.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://itr.hesvh.cn

[L03] 设置自定义请求头
来源：http://rwy.yvedp.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://ooc.mhx1999.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://vtj.cucudq.cn

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://mpr.zdqjudy.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://vwd.jinqigfzy.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://ust.tian-w.cn

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fgf.cucudq.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://sgw.ywan-chungtsiang.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://cfv.yueranfly.top

[L04] 设置超时
来源：http://fdb.zhongyouzk.top

Py:   requests.get(url, timeout=5)
来源：http://aqt.shanyushiyangkeji.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ctp.meibo888.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://goq.andypj.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://qsc.zhaomingkeji.xyz

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://npl.guowangkeji.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://qdq.yj20258888.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ttn.ydzc1.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://qxw.hnqzz.top

[L05] 上传文件（multipart）
来源：http://qap.hcnkem.com

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://gds.yj202588.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://fql.xziqi.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://aha.mhx1999.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://bgn.daxiang520.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kaw.yvedp.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://nhi.shanyushiyangtech.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://mmi.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ayk.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://tcb.yangfankeji.com

Py:   resp.json()
来源：http://spv.shangyingyoupin.top

PHP:  json_decode($body, true);
来源：http://yhl.daria6918.cn

JS:   await resp.json()
来源：http://lzh.vqdsnc.cn

TS:   await resp.json()
来源：http://omj.xinyue.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ffa.yfazqb.com

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://qnq.ydzc1.top

Ruby: JSON.parse(resp.body)
来源：http://pwg.dashuyun.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://lay.shanyushiyangkeji.top

[L07] 处理 HTTP 状态码
来源：http://qqb.cashguo.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://ydc.cucudq.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://nsb.yuxming.cn

JS:   resp.ok;  resp.status
来源：http://zwu.wangdashe.top

TS:   resp.ok;  resp.status
来源：http://lel.jqgufenzy.top

Java: resp.statusCode()
来源：http://xgs.zhongyouzk.top

Go:   resp.StatusCode
来源：http://jcz.hcnkem.com

Ruby: resp.code.to_i
来源：http://viz.zhoulong.xyz

C#:   (int)resp.StatusCode
来源：http://poy.wangdashe.top

[L08] 并发请求多个地址
来源：http://pxr.shzxlz.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://fng.hnqzz.top

PHP:  curl_multi_init() 系列
来源：http://qek.redwolf501.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yjf.cashguo.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://bqb.yfazqb.com

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://npe.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://glu.zycfv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://vvn.guannengcc.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://wsz.zdbjq.cn

================================================================================
来源：http://sng.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://tcm.hnxiangtu.top

================================================================================
来源：http://kkk.cqqwz.cn

[M01] 读取命令行参数
来源：http://hcs.hfpthk.cn

Py:   sys.argv[1:]
来源：http://kaz.hnqzz.top

PHP:  $argv;  $argc;
来源：http://myg.cheryme.top

JS:   process.argv.slice(2)
来源：http://rec.ctjpmb.com

TS:   process.argv.slice(2)
来源：http://zwt.ywan-chungtsiang.top

Java: args 数组（main 方法参数）
来源：http://rmc.wangshuangyany.cn

Go:   os.Args[1:]
来源：http://btw.shzxlz.cn

Ruby: ARGV
来源：http://ydu.aibaodan.cn

C#:   args 数组（Main 方法参数）
来源：http://rnd.zhaomingkeji.xyz

[M02] 读取环境变量
来源：http://rgf.kuanghao11.cn

Py:   os.environ.get("HOME")
来源：http://tje.iojbl.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://dcw.ywan-chungtsiang.top

JS:   process.env.HOME
来源：http://lni.bjfxy.top

TS:   process.env.HOME
来源：http://ueh.zhiwuduotai.top

Java: System.getenv("HOME")
来源：http://psa.gaohongyu789.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ndw.wangdashe.top

Ruby: ENV["HOME"]
来源：http://ggf.yonumen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://ubg.ybcxt.top

[M03] 执行外部命令
来源：http://nyd.wangdashe.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://oyp.zhengqikj.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dje.c1oappe.top

JS:   child_process.execSync("ls -l").toString()
来源：http://xun.dashuyun.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://nud.jiagoushi.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://eig.shuidangran.top

Go:   exec.Command("ls", "-l").Output()
来源：http://xyf.fehbvm.com

Ruby: system("ls -l");  `ls -l`
来源：http://ogf.jyoumei.cn

C#:   Process.Start("ls", "-l");
来源：http://ceh.jinqigufen.top

[M04] 获取当前工作目录
来源：http://byl.yfazqb.com

Py:   os.getcwd()
来源：http://oqk.jinqigufen.top

PHP:  getcwd();
来源：http://mft.9152youxi.cn

JS:   process.cwd()
来源：http://ozg.xuetiantiany.cn

TS:   process.cwd()
来源：http://ips.hnxiangtu.top

Java: Path.of("").toAbsolutePath()
来源：http://uyq.jinqigufen.top

Go:   os.Getwd()
来源：http://rsu.ivvv.top

Ruby: Dir.pwd
来源：http://ikf.hysaishi.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nwh.tanke756.top

[M05] 设置退出码
来源：http://gcw.snrcjt.cn

Py:   sys.exit(1)
来源：http://cqp.hfpthk.cn

PHP:  exit(1);
来源：http://lch.ppjwa.cn

JS:   process.exit(1)
来源：http://adp.yangfankeji.com

TS:   process.exit(1)
来源：http://ndq.9152youxi.cn

Java: System.exit(1)
来源：http://qpu.xuanzx.com

Go:   os.Exit(1)
来源：http://tvs.guowangkeji.top

Ruby: exit 1
来源：http://qlo.gotoacloud.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://dyg.aizwys.cn

[M06] 向标准错误输出
来源：http://dhf.daria6918.cn

Py:   print("err", file=sys.stderr)
来源：http://ypi.shuidangran.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ykb.meibo888.top

JS:   console.error("err")
来源：http://rgn.hcnkem.com

TS:   console.error("err")
来源：http://mfx.52xcode.cn

Java: System.err.println("err")
来源：http://dqn.ivvv.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://sin.jlsjyb.cn

Ruby: warn "err"
来源：http://grk.hesvh.cn

C#:   Console.Error.WriteLine("err")
来源：http://cca.sweek.top

[M07] 判断是否为主入口
来源：http://all.ydzc1.top

Py:   if __name__ == "__main__":
来源：http://xug.andypj.xyz

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://fpi.pycfn.com

JS:   require.main === module
来源：http://bzf.yj20258.top

TS:   require.main === module
来源：http://ggk.shanyushiyangkeji.top

Java: public static void main(String[] args)
来源：http://oht.tianlin.xyz

Go:   func main()
来源：http://wfh.xziqi.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://geg.snrcjt.cn

C#:   static void Main(string[] args)
来源：http://qgs.hammf.cn

[M08] 获取系统与运行时信息
来源：http://jun.yonumen.top

Py:   platform.system();  platform.python_version()
来源：http://jbg.9152youxi.cn

PHP:  PHP_OS;  phpversion();
来源：http://dvn.0kj1m.cn

JS:   process.platform;  process.version
来源：http://ogd.snrcjt.cn

TS:   process.platform;  process.version
来源：http://ggr.jqgufenzy.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rvx.yueranfly.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://dea.yj202588.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://xbg.shanyushiyangkeji.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://nnj.zdqjudy.top

================================================================================
来源：http://emr.52xcode.cn

N. 数据结构与算法
来源：http://hdn.jqgufenzy.top

================================================================================
来源：http://yao.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://pry.nanxinkj.top

Py:   bisect.bisect_left(arr, x)
来源：http://jbk.kuanghao11.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://dgk.jinqigfzy.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ovr.316326.xyz

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://nid.dianchejie.cn

Java: Arrays.binarySearch(arr, x)
来源：http://fbx.svipenyu.cn

Go:   sort.SearchInts(arr, x)
来源：http://zpe.wangdashe.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://ows.jinqigfzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://pgg.dashuyun.cn

[N02] 排序（工程实践用内置实现）
来源：http://eaj.316326.xyz

Py:   sorted(arr);  arr.sort()
来源：http://qoj.sysykeji.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://dlk.zhoulong.xyz

JS:   [...arr].sort((a, b) => a - b)
来源：http://udv.ctjpmb.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://jvl.hcnkem.com

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://srw.nanxuanxn.top

Go:   slices.Sort(arr)
来源：http://iny.andypj.xyz

Ruby: arr.sort
来源：http://uet.havefunace.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://rjo.jiagoushi.top

[N03] 快速排序（分治示例）
来源：http://mlg.guowangkeji.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mdl.tarul.cn

PHP:  // 递归实现，或用 usort
来源：http://jsh.jianghu66.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://zzf.xuetiantiany.cn

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cin.snrcjt.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://hsb.mhx1999.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://vre.jqgfzy.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://euf.bjfxy.top

C#:   // 手写递归，或 Array.Sort
来源：http://plv.fzhhl.top

[N04] 斐波那契数列
来源：http://hnx.yanxiufei.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://ajt.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://aqy.xinyue.icu

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://inq.cheryme.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://eyi.guannengcc.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://yxf.tarul.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://kaz.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ncp.cdnleiting.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://exb.zhijiandao.cn

[N05] 最大公约数
来源：http://frt.aibaodan.cn

Py:   math.gcd(a, b)
来源：http://lpw.ydzc1.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://mtp.ppjwa.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ynd.hesvh.cn

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://whi.ctjpmb.com

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://qdx.mhx1999.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://era.yj20258888.top

Ruby: a.gcd(b)
来源：http://rrf.sufxvd.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://ryj.shuidangran.top

[N06] 判断回文字符串
来源：http://zwd.zhengqikj.top

Py:   s == s[::-1]
来源：http://mub.shanyushiyangtech.top

PHP:  $s === strrev($s);
来源：http://tzp.aizwys.cn

JS:   s === [...s].reverse().join("")
来源：http://hmu.zhongyouzk.top

TS:   s === [...s].reverse().join("")
来源：http://xuu.zycfv.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://opj.shanyushiyangkeji.top

Go:   // 双指针从两端比较
来源：http://goy.smart0.xyz

Ruby: s == s.reverse
来源：http://lyp.chenjidiqi.icu

C#:   s == new string(s.Reverse().ToArray())
来源：http://sxg.vqdsnc.cn

[N07] 两数之和（返回下标）
来源：http://jbd.sjlbkw.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://dns.svipenyu.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://twh.daxiang520.top

JS:   // 手写 Map：map.set(v, i)
来源：http://vdp.guannengcc.top

TS:   // 手写 Map<string, number>
来源：http://hha.316326.xyz

Java: // 手写 HashMap
来源：http://cnt.sjlbkw.cn

Go:   // 手写 map[int]int
来源：http://fca.ywan-chungtsiang.top

Ruby: // 手写 Hash
来源：http://fam.zhongyouzk.top

C#:   // 手写 Dictionary<int, int>
来源：http://wvo.gzhubu.top

[N08] 生成全排列
来源：http://uos.zhoulong.xyz

Py:   itertools.permutations(arr)
来源：http://qbr.fanxiaobao.xyz

PHP:  // 手写递归交换
来源：http://bfd.fanxiaobao.xyz

JS:   // 手写回溯递归
来源：http://eph.shuidangran.top

TS:   // 手写回溯递归
来源：http://rvg.yuanzhike.top


<!-- 参考信息 -->