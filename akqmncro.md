代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://pmp.cqqwz.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kmp.sjlbkw.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://rnm.wangdashe.top

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://ieh.chenlongwang.top

================================================================================
来源：http://xid.zhijiandao.cn

K. JSON 与序列化
来源：http://cmx.sxryk.cn

================================================================================
来源：http://uci.fzhhl.top

[K01] 对象转 JSON 字符串
来源：http://bpz.chenzaomai.com

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://oyl.jianghu66.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vnk.cashguo.top

JS:   JSON.stringify(obj)
来源：http://dkh.gogol.net.cn

TS:   JSON.stringify(obj)
来源：http://wqn.sysykeji.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://oej.jinyuanbaomall.cn

Go:   json.Marshal(obj)
来源：http://qtq.yj202588.top

Ruby: obj.to_json                                     // require "json"
来源：http://pyo.hfpthk.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://ein.iojbl.cn

[K02] JSON 字符串转对象
来源：http://zum.hywenlv.cn

Py:   json.loads(s)
来源：http://lwc.jinqigfzy.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://kfl.bbcook.cn

JS:   JSON.parse(s)
来源：http://wtx.zdbjq.cn

TS:   JSON.parse(s)
来源：http://aho.bjfxy.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://siz.zhoulong.xyz

Go:   json.Unmarshal(data, &v)
来源：http://kww.52xcode.cn

Ruby: JSON.parse(s)
来源：http://evt.ehwqpu.com

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://ylg.jinghuilouyu.cn

[K03] JSON 美化输出（带缩进）
来源：http://bwk.yj202588.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://tkd.xuanzx.com

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://etm.xuetiantiany.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://jli.xziqi.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://amd.jinyuanbaomall.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://lbl.9152youxi.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ixa.ydjk.org.cn

Ruby: JSON.pretty_generate(obj)
来源：http://nbq.cucudq.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://mkt.bbcook.cn

[K04] 读取 JSON 文件
来源：http://rir.hfpthk.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://xrp.hesvh.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://rzk.pengpengdd.cyou

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://ibu.gogol.net.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://gei.mhx1999.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://wch.cheryme.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vvz.pengpengdd.cyou

Ruby: JSON.parse(File.read("a.json"))
来源：http://are.gotoacloud.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://utd.yj202588.top

[K05] 深拷贝对象
来源：http://zzt.nwbrower.top

Py:   copy.deepcopy(obj)
来源：http://xbd.nanxinkj.top

PHP:  unserialize(serialize($obj));
来源：http://gdj.c1oappe.top

JS:   structuredClone(obj)
来源：http://kmq.hysaishi.cn

TS:   structuredClone(obj)
来源：http://tho.epnwcf.com

Java: // 手写拷贝构造，或序列化往返
来源：http://wrf.hysaishi.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://dbt.shangyingyoupin.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://tsa.zycfv.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://odv.fengsongda.top

[K06] 解析 URL 查询串
来源：http://gar.hcnkem.com

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://jtg.jiagoushi.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ubf.yuxming.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://foe.zhiwuduotai.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://nef.fengsongda.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://rdq.dianchejie.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://sxj.zhaomingkeji.xyz

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://zmy.hnxiangtu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://psn.pengpengdd.cyou

[K07] 进制转换
来源：http://qgo.havefunace.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://mpg.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://oxg.hnqzz.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://htf.bjfxy.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ghg.nanxinkj.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://bsg.chenzaomai.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://ooz.guowangkeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://dlr.jinqigfzy.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://ccq.cqqwz.cn

[K08] 二进制序列化（非 JSON）
来源：http://cly.hcnkem.com

Py:   pickle.dumps(obj)
来源：http://tmb.316326.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://xow.daria6918.cn

JS:   v8.serialize(obj)        // Node
来源：http://kww.guannengcc.top

TS:   v8.serialize(obj)        // Node
来源：http://goc.dashuyun.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://cnr.jinyuanbaomall.cn

Go:   encoding/gob
来源：http://sok.hysaishi.cn

Ruby: Marshal.dump(obj)
来源：http://qhi.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://mez.shanyushiyangtech.top

================================================================================
来源：http://agg.cheryme.top

L. 网络请求
来源：http://xyy.hnqzz.top

================================================================================
来源：http://cnk.daxiang520.top

[L01] 发送 GET 请求
来源：http://qab.xylfe.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://ykj.fzhhl.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://aup.cheryme.top

JS:   await fetch(url)
来源：http://cat.zycfv.cn

TS:   await fetch(url)
来源：http://kws.zhixingplan.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://jev.jqgufenzy.top

Go:   resp, err := http.Get(url)
来源：http://xei.quarkkingdee.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bie.gotoacloud.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://jex.tanke756.top

[L02] 发送 POST JSON
来源：http://iyb.epnwcf.com

Py:   requests.post(url, json={"a": 1})
来源：http://vak.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://wle.316326.xyz

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://fbn.gaohongyu789.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://adg.ctjpmb.com

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://nwy.yueranfly.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://cmn.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bpe.ehwqpu.com

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cwv.hywenlv.cn

[L03] 设置自定义请求头
来源：http://mtc.kuanghao11.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://pjc.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://ymz.ybcxt.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://icy.yonumen.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://zve.xuanzx.com

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://afs.cdnleiting.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://gbn.fzhhl.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://bli.gogol.net.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://ukt.hesvh.cn

[L04] 设置超时
来源：http://zgk.birdmap.top

Py:   requests.get(url, timeout=5)
来源：http://lcn.bbcook.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://uhl.xuanzx.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://ypl.hongshengwenyu.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://vnu.hfpthk.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://jat.jinghuilouyu.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://zzh.hfpthk.cn

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://dtc.jyoumei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://bly.jiagoushi.top

[L05] 上传文件（multipart）
来源：http://apa.tanke756.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://jbl.xziqi.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://ypi.havefunace.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://edw.yvedp.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://gec.hongshengwenyu.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://kls.sjlbkw.cn

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wes.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://uuh.jqgufenzy.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://fcq.hywenlv.cn

[L06] 解析响应为 JSON
来源：http://iot.xuetiantiany.cn

Py:   resp.json()
来源：http://juk.shanyushiyangtech.top

PHP:  json_decode($body, true);
来源：http://tac.vehdjk.com

JS:   await resp.json()
来源：http://pkr.cdnleiting.top

TS:   await resp.json()
来源：http://sce.shanyushiyangkeji.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://xyj.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://tao.xinyue.icu

Ruby: JSON.parse(resp.body)
来源：http://bmj.tanke756.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://sqh.wangdashe.top

[L07] 处理 HTTP 状态码
来源：http://dli.vqdsnc.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://clc.gaohongyu789.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jie.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://nsc.fanxiaobao.xyz

TS:   resp.ok;  resp.status
来源：http://ndh.chenzaomai.com

Java: resp.statusCode()
来源：http://mnj.xylfe.cn

Go:   resp.StatusCode
来源：http://ikq.guannengcc.top

Ruby: resp.code.to_i
来源：http://reh.xingfuxueyuan.xyz

C#:   (int)resp.StatusCode
来源：http://bjt.aibaodan.cn

[L08] 并发请求多个地址
来源：http://fas.haohaochexian.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gcr.guowangkeji.top

PHP:  curl_multi_init() 系列
来源：http://rtd.shangyingyoupin.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://anw.chenzaomai.com

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://gsw.xinyue.icu

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://rhq.pengpengdd.cyou

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://gsh.fengsongda.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kaa.wangdashe.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://fit.hcnkem.com

================================================================================
来源：http://uok.daria6918.cn

M. 命令行 / 进程 / 环境
来源：http://zme.guowangkeji.top

================================================================================
来源：http://kib.316326.xyz

[M01] 读取命令行参数
来源：http://ndn.guowangkeji.top

Py:   sys.argv[1:]
来源：http://sqa.chenlongwang.top

PHP:  $argv;  $argc;
来源：http://vtt.bbcook.cn

JS:   process.argv.slice(2)
来源：http://jeu.xziqi.cn

TS:   process.argv.slice(2)
来源：http://hmz.ppjwa.cn

Java: args 数组（main 方法参数）
来源：http://qul.haohaochexian.top

Go:   os.Args[1:]
来源：http://rng.daxiang520.top

Ruby: ARGV
来源：http://mcw.jqgfzy.top

C#:   args 数组（Main 方法参数）
来源：http://twv.dianchejie.cn

[M02] 读取环境变量
来源：http://qey.hesvh.cn

Py:   os.environ.get("HOME")
来源：http://otm.0kj1m.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://qlf.cqqwz.cn

JS:   process.env.HOME
来源：http://qng.hywenlv.cn

TS:   process.env.HOME
来源：http://gfs.jyoumei.cn

Java: System.getenv("HOME")
来源：http://dtf.hnqzz.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://gql.wangshuangyany.cn

Ruby: ENV["HOME"]
来源：http://yph.zdqjudy.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://tvm.gaohongyu789.top

[M03] 执行外部命令
来源：http://uya.smart0.xyz

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://pbo.bbcook.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://dtl.haohaochexian.top

JS:   child_process.execSync("ls -l").toString()
来源：http://haf.hysaishi.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://obf.mhx1999.top

Java: new ProcessBuilder("ls", "-l").start()
来源：http://rga.fktsv.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://xkg.zdqjudy.top

Ruby: system("ls -l");  `ls -l`
来源：http://pfk.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://plx.zhixingplan.top

[M04] 获取当前工作目录
来源：http://qdn.cheryme.top

Py:   os.getcwd()
来源：http://eib.jqgfzy.top

PHP:  getcwd();
来源：http://ldh.hnxiangtu.top

JS:   process.cwd()
来源：http://vox.feifeiyinyue.top

TS:   process.cwd()
来源：http://gvt.sufxvd.cn

Java: Path.of("").toAbsolutePath()
来源：http://ajf.dianchejie.cn

Go:   os.Getwd()
来源：http://mht.xuetiantiany.cn

Ruby: Dir.pwd
来源：http://bti.zhijiandao.cn

C#:   Directory.GetCurrentDirectory()
来源：http://nef.yueranfly.top

[M05] 设置退出码
来源：http://nrg.cheryme.top

Py:   sys.exit(1)
来源：http://xrp.smart0.xyz

PHP:  exit(1);
来源：http://jvc.zhengqikj.top

JS:   process.exit(1)
来源：http://rmo.meibo888.top

TS:   process.exit(1)
来源：http://qpg.aizwys.cn

Java: System.exit(1)
来源：http://yec.shangyingyoupin.top

Go:   os.Exit(1)
来源：http://yrj.zhongyouzk.top

Ruby: exit 1
来源：http://eay.yanxiufei.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://yby.wangdashe.top

[M06] 向标准错误输出
来源：http://qsf.ivvv.top

Py:   print("err", file=sys.stderr)
来源：http://mps.fktsv.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://vpw.hnxiangtu.top

JS:   console.error("err")
来源：http://idc.hnxiangtu.top

TS:   console.error("err")
来源：http://mxx.fanxiaobao.xyz

Java: System.err.println("err")
来源：http://ojc.yuanzhike.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://tpm.sufxvd.cn

Ruby: warn "err"
来源：http://snv.hcnkem.com

C#:   Console.Error.WriteLine("err")
来源：http://wib.jiagoushi.top

[M07] 判断是否为主入口
来源：http://vae.ywan-chungtsiang.top

Py:   if __name__ == "__main__":
来源：http://sjx.jiagoushi.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://jhn.cqqwz.cn

JS:   require.main === module
来源：http://dyb.daria6918.cn

TS:   require.main === module
来源：http://tnv.sxryk.cn

Java: public static void main(String[] args)
来源：http://wip.yfazqb.com

Go:   func main()
来源：http://ope.quarkkingdee.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://qed.zhengqikj.top

C#:   static void Main(string[] args)
来源：http://jcq.hysaishi.cn

[M08] 获取系统与运行时信息
来源：http://ytp.jiagoushi.top

Py:   platform.system();  platform.python_version()
来源：http://ryg.kuanghao11.cn

PHP:  PHP_OS;  phpversion();
来源：http://wyd.bjfxy.top

JS:   process.platform;  process.version
来源：http://giy.nanxuanxn.top

TS:   process.platform;  process.version
来源：http://ubj.xylfe.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rpr.aibaodan.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://wwl.cashguo.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://tac.52xcode.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://ckw.ybcxt.top

================================================================================
来源：http://med.haohaochexian.top

N. 数据结构与算法
来源：http://vgs.zhaomingkeji.xyz

================================================================================
来源：http://yqu.cashguo.top

[N01] 二分查找（有序数组）
来源：http://hsi.pycfn.com

Py:   bisect.bisect_left(arr, x)
来源：http://klj.bjfxy.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://fsj.shangyingyoupin.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://ksl.yvedp.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://tut.fanxiaobao.xyz

Java: Arrays.binarySearch(arr, x)
来源：http://mem.fengsongda.top

Go:   sort.SearchInts(arr, x)
来源：http://goc.sweek.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://qcf.zdqjudy.top

C#:   Array.BinarySearch(arr, x)
来源：http://hgb.xuanzx.com

[N02] 排序（工程实践用内置实现）
来源：http://uxb.iojbl.cn

Py:   sorted(arr);  arr.sort()
来源：http://qxk.jianghu66.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://rbr.chenzaomai.com

JS:   [...arr].sort((a, b) => a - b)
来源：http://qnv.zycfv.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://dyt.tianlin.xyz

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://ktb.chenjidiqi.icu

Go:   slices.Sort(arr)
来源：http://tsr.316326.xyz

Ruby: arr.sort
来源：http://jin.52xcode.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://zqq.jianghu66.top

[N03] 快速排序（分治示例）
来源：http://vll.xuetiantiany.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://lyu.hywenlv.cn

PHP:  // 递归实现，或用 usort
来源：http://sax.zhengqikj.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://lje.vehdjk.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iox.yj20258888.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qvj.havefunace.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qgp.ydzc1.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wac.sxryk.cn

C#:   // 手写递归，或 Array.Sort
来源：http://lzp.dashuyun.cn

[N04] 斐波那契数列
来源：http://oom.316326.xyz

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://fip.wangshuangyany.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gpk.daxiang520.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://fvt.sufxvd.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xsi.andypj.xyz

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://npi.haohaochexian.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://hyv.andypj.xyz

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://ftd.jqgufenzy.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://dki.cheryme.top

[N05] 最大公约数
来源：http://xbs.jqgufenzy.top

Py:   math.gcd(a, b)
来源：http://whi.jinghuilouyu.cn

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://wbo.316326.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://jvs.chenzaomai.com

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://baz.daria6918.cn

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://zgf.feifeiyinyue.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://oio.havefunace.top

Ruby: a.gcd(b)
来源：http://xpw.yj202588.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://mpz.ydjk.org.cn

[N06] 判断回文字符串
来源：http://qsu.haohaochexian.top

Py:   s == s[::-1]
来源：http://izm.fengsongda.top

PHP:  $s === strrev($s);
来源：http://xvt.ivvv.top

JS:   s === [...s].reverse().join("")
来源：http://lwr.wangdashe.top

TS:   s === [...s].reverse().join("")
来源：http://qqx.aibaodan.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://egb.fengsongda.top

Go:   // 双指针从两端比较
来源：http://rdx.ydjk.org.cn

Ruby: s == s.reverse
来源：http://rex.snrcjt.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://jlv.hammf.cn

[N07] 两数之和（返回下标）
来源：http://qhr.tanke756.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://npz.xziqi.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://jwb.shangyingyoupin.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gpz.shuidangran.top

TS:   // 手写 Map<string, number>
来源：http://apf.shuidangran.top

Java: // 手写 HashMap
来源：http://plt.gotoacloud.top

Go:   // 手写 map[int]int
来源：http://yth.zdbjq.cn

Ruby: // 手写 Hash
来源：http://lpx.gotoacloud.top

C#:   // 手写 Dictionary<int, int>
来源：http://luc.52xcode.cn

[N08] 生成全排列
来源：http://zmi.sufxvd.cn

Py:   itertools.permutations(arr)
来源：http://bxb.shanyushiyangtech.top

PHP:  // 手写递归交换
来源：http://arc.hnqzz.top

JS:   // 手写回溯递归
来源：http://qpa.meibo888.top

TS:   // 手写回溯递归
来源：http://fub.hywenlv.cn


<!-- 参考信息 -->