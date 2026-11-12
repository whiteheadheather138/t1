代发 wailian999

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://bzq.xuanzx.com

Go:   json.Marshal(obj)
来源：http://cfp.zhongyouzk.top

Ruby: obj.to_json                                     // require "json"
来源：http://zar.xinyue.icu

C#:   JsonSerializer.Serialize(obj)
来源：http://ecg.yfazqb.com

[K02] JSON 字符串转对象
来源：http://rhi.vehdjk.com

Py:   json.loads(s)
来源：http://wgd.haohaochexian.top

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://hfw.sjlbkw.cn

JS:   JSON.parse(s)
来源：http://snu.uphjek.com

TS:   JSON.parse(s)
来源：http://pbl.xuetiantiany.cn

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://huq.ppjwa.cn

Go:   json.Unmarshal(data, &v)
来源：http://lwp.cqqwz.cn

Ruby: JSON.parse(s)
来源：http://ztw.zhijiandao.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://imv.hcnkem.com

[K03] JSON 美化输出（带缩进）
来源：http://qac.jinqigufen.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://xgz.jinyuanbaomall.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://alb.feifeiyinyue.top

JS:   JSON.stringify(obj, null, 2)
来源：http://suq.snrcjt.cn

TS:   JSON.stringify(obj, null, 2)
来源：http://xje.jlsjyb.cn

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://bvq.iojbl.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://emr.jinghuilouyu.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zaf.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://kxd.guannengcc.top

[K04] 读取 JSON 文件
来源：http://cje.jlsjyb.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://icq.shzxlz.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://agd.tianlin.xyz

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://das.ehwqpu.com

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kse.fanxiaobao.xyz

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://mkr.fktsv.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://ddo.hysaishi.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://pvy.jinghuilouyu.cn

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://bma.aizwys.cn

[K05] 深拷贝对象
来源：http://glt.andypj.xyz

Py:   copy.deepcopy(obj)
来源：http://etv.shanyushiyangtech.top

PHP:  unserialize(serialize($obj));
来源：http://pdd.hnqzz.top

JS:   structuredClone(obj)
来源：http://xqv.c1oappe.top

TS:   structuredClone(obj)
来源：http://wdd.zhixingplan.top

Java: // 手写拷贝构造，或序列化往返
来源：http://aky.xinyue.icu

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://hje.iojbl.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://hhd.meibo888.top

C#:   // 序列化往返，或自定义 Clone
来源：http://jme.guannengcc.top

[K06] 解析 URL 查询串
来源：http://tjd.yueranfly.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://lje.jinqigfzy.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pub.meibo888.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://jxh.jiagoushi.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://bsm.hnqzz.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ypn.jlsjyb.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://xbl.zdbjq.cn

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://pfo.ehwqpu.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://uqj.hcnkem.com

[K07] 进制转换
来源：http://scb.daxiang520.top

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://bvs.shzxlz.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://iiz.yvedp.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://mfq.vehdjk.com

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://ojk.gzhubu.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://lid.fktsv.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://vzr.bjfxy.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://ucl.yj20258.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://fow.bjfxy.top

[K08] 二进制序列化（非 JSON）
来源：http://knd.fengsongda.top

Py:   pickle.dumps(obj)
来源：http://dmx.tianlin.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ygi.xingfuxueyuan.xyz

JS:   v8.serialize(obj)        // Node
来源：http://mnd.c1oappe.top

TS:   v8.serialize(obj)        // Node
来源：http://klc.chenzaomai.com

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://esj.hesvh.cn

Go:   encoding/gob
来源：http://dbh.yangfankeji.com

Ruby: Marshal.dump(obj)
来源：http://mjq.fzhhl.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bmc.sufxvd.cn

================================================================================
来源：http://rrp.hcnkem.com

L. 网络请求
来源：http://taa.cheryme.top

================================================================================
来源：http://jru.chenlongwang.top

[L01] 发送 GET 请求
来源：http://bni.316326.xyz

Py:   requests.get(url)                        # 第三方库 requests
来源：http://dzb.nanxinkj.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://pkc.aibaodan.cn

JS:   await fetch(url)
来源：http://uso.jinqigfzy.top

TS:   await fetch(url)
来源：http://fpd.cqqwz.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://nev.yuxming.cn

Go:   resp, err := http.Get(url)
来源：http://olq.hnqzz.top

Ruby: Net::HTTP.get(URI(url))
来源：http://bsc.dashuyun.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tuq.yj20258.top

[L02] 发送 POST JSON
来源：http://oyl.ehwqpu.com

Py:   requests.post(url, json={"a": 1})
来源：http://nai.xingfuxueyuan.xyz

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://rfu.yvedp.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://yiy.iojbl.cn

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://pld.ivvv.top

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://ldm.nanxinkj.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://bve.ydjk.org.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://hlr.9152youxi.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://cvn.yj20258.top

[L03] 设置自定义请求头
来源：http://xnu.gzhubu.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://tnt.hnxiangtu.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://mqk.chenjidiqi.icu

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://cwj.yuxming.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://xur.gotoacloud.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://fot.yfazqb.com

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://uoj.hongshengwenyu.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://eic.ydjk.org.cn

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://hlx.guowangkeji.top

[L04] 设置超时
来源：http://dqx.dashuyun.cn

Py:   requests.get(url, timeout=5)
来源：http://fpt.gaohongyu789.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://zzj.jyoumei.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://xqt.sweek.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://uzn.chenjidiqi.icu

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://rwu.jinqigfzy.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://xwr.birdmap.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fhg.jinghuilouyu.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://stl.yongpay.top

[L05] 上传文件（multipart）
来源：http://dfr.jinqigfzy.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://dyt.chenjidiqi.icu

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://vic.ehwqpu.com

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://yqr.hnqzz.top

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://ymp.c1oappe.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://ujm.zhaomingkeji.xyz

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://prr.tianlin.xyz

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://zvg.cheryme.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://wqs.svipenyu.cn

[L06] 解析响应为 JSON
来源：http://yzu.ydzc1.top

Py:   resp.json()
来源：http://dpl.redwolf501.top

PHP:  json_decode($body, true);
来源：http://pmf.hnxiangtu.top

JS:   await resp.json()
来源：http://ntj.shanyushiyangtech.top

TS:   await resp.json()
来源：http://brh.mhx1999.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://ict.hfpthk.cn

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://myp.birdmap.top

Ruby: JSON.parse(resp.body)
来源：http://fvu.316326.xyz

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qxi.gogol.net.cn

[L07] 处理 HTTP 状态码
来源：http://wke.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://rew.shanyushiyangkeji.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://sof.guowangkeji.top

JS:   resp.ok;  resp.status
来源：http://uqw.0kj1m.cn

TS:   resp.ok;  resp.status
来源：http://wln.shangyingyoupin.top

Java: resp.statusCode()
来源：http://ech.havefunace.top

Go:   resp.StatusCode
来源：http://fob.guowangkeji.top

Ruby: resp.code.to_i
来源：http://dxn.zhixingplan.top

C#:   (int)resp.StatusCode
来源：http://qkx.yfazqb.com

[L08] 并发请求多个地址
来源：http://xab.guowangkeji.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://ekv.feifeiyinyue.top

PHP:  curl_multi_init() 系列
来源：http://xpu.hammf.cn

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://kdw.zhijiandao.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vcm.zhongyouzk.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://qze.ctjpmb.com

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://vdh.pengpengdd.cyou

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://rfw.yj20258888.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://emz.hongshengwenyu.top

================================================================================
来源：http://jlr.feifeiyinyue.top

M. 命令行 / 进程 / 环境
来源：http://gbe.jinqigfzy.top

================================================================================
来源：http://uki.tanke756.top

[M01] 读取命令行参数
来源：http://iim.ywan-chungtsiang.top

Py:   sys.argv[1:]
来源：http://jeo.gaohongyu789.top

PHP:  $argv;  $argc;
来源：http://xfs.hysaishi.cn

JS:   process.argv.slice(2)
来源：http://par.hnxiangtu.top

TS:   process.argv.slice(2)
来源：http://kir.chenjidiqi.icu

Java: args 数组（main 方法参数）
来源：http://ouf.tanke756.top

Go:   os.Args[1:]
来源：http://zvk.chenzaomai.com

Ruby: ARGV
来源：http://exc.yuxming.cn

C#:   args 数组（Main 方法参数）
来源：http://pbs.tianlin.xyz

[M02] 读取环境变量
来源：http://bab.fehbvm.com

Py:   os.environ.get("HOME")
来源：http://ipb.jiagoushi.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://lwo.ybcxt.top

JS:   process.env.HOME
来源：http://qlu.chenjidiqi.icu

TS:   process.env.HOME
来源：http://pdd.hfpthk.cn

Java: System.getenv("HOME")
来源：http://ajb.redwolf501.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nmg.xuanzx.com

Ruby: ENV["HOME"]
来源：http://bhu.jinqigufen.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://fsl.xingfuxueyuan.xyz

[M03] 执行外部命令
来源：http://ijo.guowangkeji.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://anr.chenjidiqi.icu

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://wyr.tanke756.top

JS:   child_process.execSync("ls -l").toString()
来源：http://aug.yj202588.top

TS:   child_process.execSync("ls -l").toString()
来源：http://fcm.xingfuxueyuan.xyz

Java: new ProcessBuilder("ls", "-l").start()
来源：http://zqs.iojbl.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://our.iojbl.cn

Ruby: system("ls -l");  `ls -l`
来源：http://bia.shanyushiyangkeji.top

C#:   Process.Start("ls", "-l");
来源：http://sqc.hcnkem.com

[M04] 获取当前工作目录
来源：http://uvd.cdnleiting.top

Py:   os.getcwd()
来源：http://wjp.daria6918.cn

PHP:  getcwd();
来源：http://ako.vqdsnc.cn

JS:   process.cwd()
来源：http://idp.yuxming.cn

TS:   process.cwd()
来源：http://miv.xinyue.icu

Java: Path.of("").toAbsolutePath()
来源：http://kdc.cashguo.top

Go:   os.Getwd()
来源：http://qcv.zhixingplan.top

Ruby: Dir.pwd
来源：http://hzo.epnwcf.com

C#:   Directory.GetCurrentDirectory()
来源：http://fep.sysykeji.top

[M05] 设置退出码
来源：http://gle.hesvh.cn

Py:   sys.exit(1)
来源：http://lvz.sweek.top

PHP:  exit(1);
来源：http://yws.yuanzhike.top

JS:   process.exit(1)
来源：http://hjf.gzhubu.top

TS:   process.exit(1)
来源：http://wbx.guannengcc.top

Java: System.exit(1)
来源：http://puk.yanxiufei.cn

Go:   os.Exit(1)
来源：http://glf.xziqi.cn

Ruby: exit 1
来源：http://qqc.yj202588.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://qeh.sxryk.cn

[M06] 向标准错误输出
来源：http://jod.daxiang520.top

Py:   print("err", file=sys.stderr)
来源：http://sbo.pycfn.com

PHP:  fwrite(STDERR, "err\n");
来源：http://ewp.ppjwa.cn

JS:   console.error("err")
来源：http://ulm.svipenyu.cn

TS:   console.error("err")
来源：http://vmp.yj20258888.top

Java: System.err.println("err")
来源：http://ybr.chenzaomai.com

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://hzq.ybcxt.top

Ruby: warn "err"
来源：http://kyp.hysaishi.cn

C#:   Console.Error.WriteLine("err")
来源：http://wui.snrcjt.cn

[M07] 判断是否为主入口
来源：http://nnu.xylfe.cn

Py:   if __name__ == "__main__":
来源：http://hpc.fehbvm.com

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lmr.wangshuangyany.cn

JS:   require.main === module
来源：http://iau.zdbjq.cn

TS:   require.main === module
来源：http://yxc.c1oappe.top

Java: public static void main(String[] args)
来源：http://ych.fktsv.cn

Go:   func main()
来源：http://plm.shanyushiyangkeji.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://mhy.bbcook.cn

C#:   static void Main(string[] args)
来源：http://orm.fehbvm.com

[M08] 获取系统与运行时信息
来源：http://kly.ppjwa.cn

Py:   platform.system();  platform.python_version()
来源：http://ogy.tianlin.xyz

PHP:  PHP_OS;  phpversion();
来源：http://vpn.zhoulong.xyz

JS:   process.platform;  process.version
来源：http://ssa.gaohongyu789.top

TS:   process.platform;  process.version
来源：http://xms.hysaishi.cn

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://qci.fengsongda.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://pxl.jinqigufen.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cqf.yonumen.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://krj.guannengcc.top

================================================================================
来源：http://zrq.yanxiufei.cn

N. 数据结构与算法
来源：http://pnb.fktsv.cn

================================================================================
来源：http://bqb.c1oappe.top

[N01] 二分查找（有序数组）
来源：http://vbo.hesvh.cn

Py:   bisect.bisect_left(arr, x)
来源：http://ess.dashuyun.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://pnw.nanxuanxn.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hwg.hysaishi.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://uii.quarkkingdee.top

Java: Arrays.binarySearch(arr, x)
来源：http://rpw.shanyushiyangtech.top

Go:   sort.SearchInts(arr, x)
来源：http://alq.jqgfzy.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://blg.jqgufenzy.top

C#:   Array.BinarySearch(arr, x)
来源：http://hmt.zdbjq.cn

[N02] 排序（工程实践用内置实现）
来源：http://hkn.andypj.xyz

Py:   sorted(arr);  arr.sort()
来源：http://bvy.cucudq.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ywy.xuetiantiany.cn

JS:   [...arr].sort((a, b) => a - b)
来源：http://hzp.epnwcf.com

TS:   [...arr].sort((a, b) => a - b)
来源：http://lnb.wangshuangyany.cn

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://imn.bbcook.cn

Go:   slices.Sort(arr)
来源：http://miw.sufxvd.cn

Ruby: arr.sort
来源：http://onj.hammf.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://soi.guowangkeji.top

[N03] 快速排序（分治示例）
来源：http://qwf.tianlin.xyz

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://nkp.316326.xyz

PHP:  // 递归实现，或用 usort
来源：http://yqg.guowangkeji.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ngv.meibo888.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://jay.cqqwz.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://vsq.nwbrower.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ipr.cdnleiting.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://wks.feifeiyinyue.top

C#:   // 手写递归，或 Array.Sort
来源：http://zlu.ehwqpu.com

[N04] 斐波那契数列
来源：http://ewj.daria6918.cn

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://wws.cdnleiting.top

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://nmo.redwolf501.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ujo.shanyushiyangkeji.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://wnz.snrcjt.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://hqr.ydzc1.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://vck.shangyingyoupin.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://peo.gaohongyu789.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ona.hnqzz.top

[N05] 最大公约数
来源：http://zok.zhiwuduotai.top

Py:   math.gcd(a, b)
来源：http://aia.shanyushiyangkeji.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://ehv.zhixingplan.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dyp.andypj.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://gxi.gaohongyu789.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://wxr.birdmap.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://shg.pengpengdd.cyou

Ruby: a.gcd(b)
来源：http://get.cqqwz.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://cof.bbcook.cn

[N06] 判断回文字符串
来源：http://eef.hysaishi.cn

Py:   s == s[::-1]
来源：http://tvk.gaohongyu789.top

PHP:  $s === strrev($s);
来源：http://gdt.nanxuanxn.top

JS:   s === [...s].reverse().join("")
来源：http://okm.zdqjudy.top

TS:   s === [...s].reverse().join("")
来源：http://knc.ehwqpu.com

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://ykf.zhaomingkeji.xyz

Go:   // 双指针从两端比较
来源：http://qci.guannengcc.top

Ruby: s == s.reverse
来源：http://anv.pycfn.com

C#:   s == new string(s.Reverse().ToArray())
来源：http://cam.jianghu66.top

[N07] 两数之和（返回下标）
来源：http://mkm.aizwys.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://lvp.guannengcc.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://ohs.hongshengwenyu.top

JS:   // 手写 Map：map.set(v, i)
来源：http://zvd.nanxinkj.top

TS:   // 手写 Map<string, number>
来源：http://uas.ydjk.org.cn

Java: // 手写 HashMap
来源：http://wuc.aizwys.cn

Go:   // 手写 map[int]int
来源：http://hke.xziqi.cn

Ruby: // 手写 Hash
来源：http://snd.fehbvm.com

C#:   // 手写 Dictionary<int, int>
来源：http://utj.yj20258888.top

[N08] 生成全排列
来源：http://ymr.yj202588.top

Py:   itertools.permutations(arr)
来源：http://gye.pycfn.com

PHP:  // 手写递归交换
来源：http://auu.quarkkingdee.top

JS:   // 手写回溯递归
来源：http://imh.svipenyu.cn

TS:   // 手写回溯递归
来源：http://skh.zycfv.cn

Java: // 手写回溯递归
来源：http://eop.hongshengwenyu.top

Go:   // 手写回溯递归
来源：http://wzc.vqdsnc.cn

Ruby: arr.permutation.to_a
来源：http://udr.zdqjudy.top

C#:   // 手写回溯递归
来源：http://qzn.daria6918.cn

[N09] 栈与队列
来源：http://byp.yj20258.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://efa.aibaodan.cn

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://idm.jianghu66.top

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://etn.hammf.cn

TS:   arr.push(x) / arr.pop() 作栈
来源：http://tcs.sweek.top

Java: new ArrayDeque<>() 同时支持栈与队列
来源：http://wdn.ybcxt.top

Go:   append(s, x) 与 s[len(s)-1] 出栈
来源：http://dvg.dianchejie.cn

Ruby: arr.push / arr.pop 作栈；arr.shift 作队列
来源：http://qso.nanxuanxn.top


<!-- 参考信息 -->