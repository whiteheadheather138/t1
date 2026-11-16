代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://wvu.jyoumei.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kru.xuetiantiany.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://kkp.yfazqb.com

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://zaq.mhx1999.top

================================================================================
来源：http://hrt.havefunace.top

K. JSON 与序列化
来源：http://tvw.havefunace.top

================================================================================
来源：http://ybm.iojbl.cn

[K01] 对象转 JSON 字符串
来源：http://shw.gzhubu.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://wlx.sxryk.cn

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://rvz.dashuyun.cn

JS:   JSON.stringify(obj)
来源：http://gvo.yangfankeji.com

TS:   JSON.stringify(obj)
来源：http://mty.yonumen.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://rul.fanxiaobao.xyz

Go:   json.Marshal(obj)
来源：http://dqn.jiagoushi.top

Ruby: obj.to_json                                     // require "json"
来源：http://lfc.gzhubu.top

C#:   JsonSerializer.Serialize(obj)
来源：http://yao.quarkkingdee.top

[K02] JSON 字符串转对象
来源：http://ieg.andypj.xyz

Py:   json.loads(s)
来源：http://nai.iojbl.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://dwe.zhijiandao.cn

JS:   JSON.parse(s)
来源：http://qdj.zhengqikj.top

TS:   JSON.parse(s)
来源：http://qpg.snrcjt.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://tvt.ydzc1.top

Go:   json.Unmarshal(data, &v)
来源：http://ima.hammf.cn

Ruby: JSON.parse(s)
来源：http://fng.yanxiufei.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://mii.zdqjudy.top

[K03] JSON 美化输出（带缩进）
来源：http://tff.0kj1m.cn

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://aco.havefunace.top

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://epd.tanke756.top

JS:   JSON.stringify(obj, null, 2)
来源：http://txs.ivvv.top

TS:   JSON.stringify(obj, null, 2)
来源：http://wot.jianghu66.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://xid.dianchejie.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://xsd.svipenyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://cct.cdnleiting.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://lgw.jinghuilouyu.cn

[K04] 读取 JSON 文件
来源：http://zbr.fzhhl.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://qxr.zhaomingkeji.xyz

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://ugr.sweek.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://vdv.shangyingyoupin.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://weg.shuidangran.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mjv.0kj1m.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://yhl.shzxlz.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://rpx.zhengqikj.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://lsg.shanyushiyangtech.top

[K05] 深拷贝对象
来源：http://zjh.quarkkingdee.top

Py:   copy.deepcopy(obj)
来源：http://huk.redwolf501.top

PHP:  unserialize(serialize($obj));
来源：http://dqh.yuxming.cn

JS:   structuredClone(obj)
来源：http://cos.cheryme.top

TS:   structuredClone(obj)
来源：http://gpr.hywenlv.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://cqf.nanxuanxn.top

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://xnk.zhijiandao.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://cui.shanyushiyangkeji.top

C#:   // 序列化往返，或自定义 Clone
来源：http://deg.fengsongda.top

[K06] 解析 URL 查询串
来源：http://ehm.snrcjt.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://dec.yj20258888.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://rpc.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://pzl.pycfn.com

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://ioc.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ikn.yfazqb.com

Go:   url.ParseQuery("a=1&b=2")
来源：http://dfb.gaohongyu789.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://ykb.kuanghao11.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://ens.zdqjudy.top

[K07] 进制转换
来源：http://amr.iojbl.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://fjo.fehbvm.com

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://kpv.yonumen.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://kwu.yj20258888.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://sgu.meibo888.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://jaq.cdnleiting.top

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://pjw.316326.xyz

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://cei.fanxiaobao.xyz

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://qof.dianchejie.cn

[K08] 二进制序列化（非 JSON）
来源：http://zyr.hammf.cn

Py:   pickle.dumps(obj)
来源：http://oac.bjfxy.top

PHP:  serialize($obj);  unserialize($s);
来源：http://ezv.zhoulong.xyz

JS:   v8.serialize(obj)        // Node
来源：http://fmy.ppjwa.cn

TS:   v8.serialize(obj)        // Node
来源：http://dgq.uphjek.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://slq.andypj.xyz

Go:   encoding/gob
来源：http://gqc.snrcjt.cn

Ruby: Marshal.dump(obj)
来源：http://lkj.hysaishi.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://qda.uphjek.com

================================================================================
来源：http://ssz.guowangkeji.top

L. 网络请求
来源：http://xte.jqgfzy.top

================================================================================
来源：http://xkg.yueranfly.top

[L01] 发送 GET 请求
来源：http://wlx.hywenlv.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://aiw.dashuyun.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://tie.pycfn.com

JS:   await fetch(url)
来源：http://xds.kuanghao11.cn

TS:   await fetch(url)
来源：http://kbd.aizwys.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://rck.sjlbkw.cn

Go:   resp, err := http.Get(url)
来源：http://lgf.hcnkem.com

Ruby: Net::HTTP.get(URI(url))
来源：http://ybi.nanxuanxn.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://hsa.aizwys.cn

[L02] 发送 POST JSON
来源：http://klw.hysaishi.cn

Py:   requests.post(url, json={"a": 1})
来源：http://grc.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://uho.tarul.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://psw.ppjwa.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://drh.yueranfly.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://xew.wangshuangyany.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://fvs.hcnkem.com

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://lxh.wangdashe.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://jst.nwbrower.top

[L03] 设置自定义请求头
来源：http://bgt.gotoacloud.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zeo.zhixingplan.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://biq.hnqzz.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://emt.smart0.xyz

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://fja.daxiang520.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hsc.meibo888.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://dry.ehwqpu.com

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://avm.fzhhl.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://psk.fzhhl.top

[L04] 设置超时
来源：http://zby.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://rnw.xinyue.icu

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://dfd.kuanghao11.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://jdn.shangyingyoupin.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://dkv.zhongyouzk.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://yod.zhoulong.xyz

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://kzw.tanke756.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://ryv.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://anq.dashuyun.cn

[L05] 上传文件（multipart）
来源：http://tcw.ywan-chungtsiang.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://wro.nanxuanxn.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://rak.yfazqb.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yue.gzhubu.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://xfi.hesvh.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zub.chenjidiqi.icu

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://xew.xinyue.icu

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://efn.tian-w.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://sho.snrcjt.cn

[L06] 解析响应为 JSON
来源：http://lpp.gaohongyu789.top

Py:   resp.json()
来源：http://iwj.haohaochexian.top

PHP:  json_decode($body, true);
来源：http://jgg.cashguo.top

JS:   await resp.json()
来源：http://qbi.jinghuilouyu.cn

TS:   await resp.json()
来源：http://bmf.c1oappe.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://kfd.wangdashe.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://jkk.fzhhl.top

Ruby: JSON.parse(resp.body)
来源：http://taw.cheryme.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://kdp.jlsjyb.cn

[L07] 处理 HTTP 状态码
来源：http://pgr.fktsv.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://aqt.fehbvm.com

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://jkx.gaohongyu789.top

JS:   resp.ok;  resp.status
来源：http://vfz.tian-w.cn

TS:   resp.ok;  resp.status
来源：http://glj.chenzaomai.com

Java: resp.statusCode()
来源：http://qac.ydjk.org.cn

Go:   resp.StatusCode
来源：http://ape.ppjwa.cn

Ruby: resp.code.to_i
来源：http://rky.pengpengdd.cyou

C#:   (int)resp.StatusCode
来源：http://vpz.yuxming.cn

[L08] 并发请求多个地址
来源：http://vxp.0kj1m.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://eig.jyoumei.cn

PHP:  curl_multi_init() 系列
来源：http://kal.fengsongda.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://don.ppjwa.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ogl.zdbjq.cn

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://coj.chenzaomai.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://ynf.aibaodan.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://bgw.xziqi.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://kjs.havefunace.top

================================================================================
来源：http://sfk.gogol.net.cn

M. 命令行 / 进程 / 环境
来源：http://reg.cashguo.top

================================================================================
来源：http://fud.ywan-chungtsiang.top

[M01] 读取命令行参数
来源：http://olq.hfpthk.cn

Py:   sys.argv[1:]
来源：http://pvd.xuetiantiany.cn

PHP:  $argv;  $argc;
来源：http://zpx.0kj1m.cn

JS:   process.argv.slice(2)
来源：http://giz.zhongyouzk.top

TS:   process.argv.slice(2)
来源：http://sgk.aizwys.cn

Java: args 数组（main 方法参数）
来源：http://zir.hywenlv.cn

Go:   os.Args[1:]
来源：http://ctb.daria6918.cn

Ruby: ARGV
来源：http://kim.zhiwuduotai.top

C#:   args 数组（Main 方法参数）
来源：http://ijs.tianlin.xyz

[M02] 读取环境变量
来源：http://nqn.havefunace.top

Py:   os.environ.get("HOME")
来源：http://pmc.fzhhl.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://tea.bbcook.cn

JS:   process.env.HOME
来源：http://uvz.jinqigfzy.top

TS:   process.env.HOME
来源：http://xcn.316326.xyz

Java: System.getenv("HOME")
来源：http://wvw.nanxinkj.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://ajb.shzxlz.cn

Ruby: ENV["HOME"]
来源：http://pxi.ywan-chungtsiang.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://hwt.nanxuanxn.top

[M03] 执行外部命令
来源：http://vdg.yfazqb.com

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://vbj.zhiwuduotai.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ntv.dashuyun.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://jje.sufxvd.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ips.xinyue.icu

Java: new ProcessBuilder("ls", "-l").start()
来源：http://vzg.zhijiandao.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://wyy.dianchejie.cn

Ruby: system("ls -l");  `ls -l`
来源：http://gxz.guannengcc.top

C#:   Process.Start("ls", "-l");
来源：http://mdi.316326.xyz

[M04] 获取当前工作目录
来源：http://vsm.svipenyu.cn

Py:   os.getcwd()
来源：http://qvw.ydjk.org.cn

PHP:  getcwd();
来源：http://tso.ivvv.top

JS:   process.cwd()
来源：http://otp.fktsv.cn

TS:   process.cwd()
来源：http://itj.ivvv.top

Java: Path.of("").toAbsolutePath()
来源：http://jiq.iojbl.cn

Go:   os.Getwd()
来源：http://aeh.yonumen.top

Ruby: Dir.pwd
来源：http://ozf.cheryme.top

C#:   Directory.GetCurrentDirectory()
来源：http://tja.dashuyun.cn

[M05] 设置退出码
来源：http://iax.cucudq.cn

Py:   sys.exit(1)
来源：http://wvl.gogol.net.cn

PHP:  exit(1);
来源：http://tme.bbcook.cn

JS:   process.exit(1)
来源：http://eay.yuxming.cn

TS:   process.exit(1)
来源：http://uzq.ywan-chungtsiang.top

Java: System.exit(1)
来源：http://xau.9152youxi.cn

Go:   os.Exit(1)
来源：http://nay.c1oappe.top

Ruby: exit 1
来源：http://hib.jinqigufen.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://uqk.shanyushiyangtech.top

[M06] 向标准错误输出
来源：http://mwf.nwbrower.top

Py:   print("err", file=sys.stderr)
来源：http://xxs.sjlbkw.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://aty.tianlin.xyz

JS:   console.error("err")
来源：http://mgs.dianchejie.cn

TS:   console.error("err")
来源：http://wwa.ybcxt.top

Java: System.err.println("err")
来源：http://zer.cqqwz.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ujk.vqdsnc.cn

Ruby: warn "err"
来源：http://vdv.hnqzz.top

C#:   Console.Error.WriteLine("err")
来源：http://gyr.sysykeji.top

[M07] 判断是否为主入口
来源：http://psr.daria6918.cn

Py:   if __name__ == "__main__":
来源：http://yjc.tian-w.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://thp.yuxming.cn

JS:   require.main === module
来源：http://uez.zdbjq.cn

TS:   require.main === module
来源：http://sgf.yueranfly.top

Java: public static void main(String[] args)
来源：http://grr.jqgfzy.top

Go:   func main()
来源：http://oin.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bgl.wangdashe.top

C#:   static void Main(string[] args)
来源：http://leb.gaohongyu789.top

[M08] 获取系统与运行时信息
来源：http://bfl.jinghuilouyu.cn

Py:   platform.system();  platform.python_version()
来源：http://fei.sysykeji.top

PHP:  PHP_OS;  phpversion();
来源：http://ldk.shanyushiyangtech.top

JS:   process.platform;  process.version
来源：http://ihh.vehdjk.com

TS:   process.platform;  process.version
来源：http://cyv.sysykeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://rhy.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://ysd.guowangkeji.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://rdh.pengpengdd.cyou

C#:   Environment.OSVersion;  Environment.Version
来源：http://ufu.0kj1m.cn

================================================================================
来源：http://rzt.cucudq.cn

N. 数据结构与算法
来源：http://kqe.mhx1999.top

================================================================================
来源：http://kue.zycfv.cn

[N01] 二分查找（有序数组）
来源：http://cad.vqdsnc.cn

Py:   bisect.bisect_left(arr, x)
来源：http://svn.chenlongwang.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://lme.ydzc1.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://sru.yonumen.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://rua.0kj1m.cn

Java: Arrays.binarySearch(arr, x)
来源：http://nzd.feifeiyinyue.top

Go:   sort.SearchInts(arr, x)
来源：http://zas.9152youxi.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://iec.guannengcc.top

C#:   Array.BinarySearch(arr, x)
来源：http://ebs.tanke756.top

[N02] 排序（工程实践用内置实现）
来源：http://gba.uphjek.com

Py:   sorted(arr);  arr.sort()
来源：http://eiz.yongpay.top

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://vww.jinqigufen.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://rzh.xingfuxueyuan.xyz

TS:   [...arr].sort((a, b) => a - b)
来源：http://qzg.ywan-chungtsiang.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://fjk.jqgufenzy.top

Go:   slices.Sort(arr)
来源：http://gob.fktsv.cn

Ruby: arr.sort
来源：http://pnh.nanxinkj.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://blv.hammf.cn

[N03] 快速排序（分治示例）
来源：http://osv.jinqigfzy.top

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://mlq.xuetiantiany.cn

PHP:  // 递归实现，或用 usort
来源：http://dpd.zhiwuduotai.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://cug.hongshengwenyu.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://mes.sxryk.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://irx.zhengqikj.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://hcm.fktsv.cn

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://bvs.epnwcf.com

C#:   // 手写递归，或 Array.Sort
来源：http://rik.wangdashe.top

[N04] 斐波那契数列
来源：http://dig.pengpengdd.cyou

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://gjp.pycfn.com

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://awj.cqqwz.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://zrw.jlsjyb.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://xxh.9152youxi.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://xge.kuanghao11.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://qyl.9152youxi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://erp.yangfankeji.com

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://kjm.ydjk.org.cn

[N05] 最大公约数
来源：http://btr.yvedp.cn

Py:   math.gcd(a, b)
来源：http://oue.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://fck.smart0.xyz

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://lmd.ydzc1.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://kza.tianlin.xyz

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://jph.xziqi.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://hrc.chenlongwang.top

Ruby: a.gcd(b)
来源：http://wie.wangdashe.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://pph.yuanzhike.top

[N06] 判断回文字符串
来源：http://chy.0kj1m.cn

Py:   s == s[::-1]
来源：http://ien.sweek.top

PHP:  $s === strrev($s);
来源：http://hmm.ctjpmb.com

JS:   s === [...s].reverse().join("")
来源：http://nbt.316326.xyz

TS:   s === [...s].reverse().join("")
来源：http://uxc.9152youxi.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://dkv.zhengqikj.top

Go:   // 双指针从两端比较
来源：http://ayq.jinqigufen.top

Ruby: s == s.reverse
来源：http://fye.jqgfzy.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://kzd.shanyushiyangkeji.top

[N07] 两数之和（返回下标）
来源：http://ebh.hnxiangtu.top

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://jnl.gogol.net.cn

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ffa.nanxuanxn.top

JS:   // 手写 Map：map.set(v, i)
来源：http://gva.pengpengdd.cyou

TS:   // 手写 Map<string, number>
来源：http://kyi.yvedp.cn

Java: // 手写 HashMap
来源：http://kxe.zhongyouzk.top

Go:   // 手写 map[int]int
来源：http://vmu.cdnleiting.top

Ruby: // 手写 Hash
来源：http://dsg.vqdsnc.cn

C#:   // 手写 Dictionary<int, int>
来源：http://bha.tanke756.top

[N08] 生成全排列
来源：http://tva.shanyushiyangkeji.top

Py:   itertools.permutations(arr)
来源：http://slc.aibaodan.cn

PHP:  // 手写递归交换
来源：http://zjc.0kj1m.cn

JS:   // 手写回溯递归
来源：http://bai.316326.xyz

TS:   // 手写回溯递归
来源：http://lms.ydjk.org.cn


<!-- 参考信息 -->