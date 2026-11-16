代发 wailian999

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://bjx.hesvh.cn

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://duy.ctjpmb.com

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://fuj.vqdsnc.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://dlu.zhaomingkeji.xyz

================================================================================
来源：http://yrh.hongshengwenyu.top

K. JSON 与序列化
来源：http://sxf.xingfuxueyuan.xyz

================================================================================
来源：http://jxb.tian-w.cn

[K01] 对象转 JSON 字符串
来源：http://mnl.jinqigfzy.top

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://yvz.yueranfly.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://igr.tarul.cn

JS:   JSON.stringify(obj)
来源：http://moi.yj20258888.top

TS:   JSON.stringify(obj)
来源：http://wya.guannengcc.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://fbe.tianlin.xyz

Go:   json.Marshal(obj)
来源：http://lzn.mhx1999.top

Ruby: obj.to_json                                     // require "json"
来源：http://vvn.316326.xyz

C#:   JsonSerializer.Serialize(obj)
来源：http://amo.xuanzx.com

[K02] JSON 字符串转对象
来源：http://ksg.dianchejie.cn

Py:   json.loads(s)
来源：http://sqn.snrcjt.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://orh.redwolf501.top

JS:   JSON.parse(s)
来源：http://iuk.yonumen.top

TS:   JSON.parse(s)
来源：http://onj.mhx1999.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://bxg.yfazqb.com

Go:   json.Unmarshal(data, &v)
来源：http://fod.daria6918.cn

Ruby: JSON.parse(s)
来源：http://nbs.dashuyun.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://cvt.xziqi.cn

[K03] JSON 美化输出（带缩进）
来源：http://qad.guannengcc.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://hqq.yanxiufei.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://evr.ppjwa.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://rls.tianlin.xyz

TS:   JSON.stringify(obj, null, 2)
来源：http://dxb.hongshengwenyu.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://eyu.yueranfly.top

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://izw.hnxiangtu.top

Ruby: JSON.pretty_generate(obj)
来源：http://klt.nanxuanxn.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://thw.cqqwz.cn

[K04] 读取 JSON 文件
来源：http://eux.316326.xyz

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://yjj.bbcook.cn

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uzd.xinyue.icu

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://dec.xinyue.icu

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zed.dianchejie.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://doc.daxiang520.top

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://mts.yj202588.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://cvo.fengsongda.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://vqg.ydjk.org.cn

[K05] 深拷贝对象
来源：http://off.tian-w.cn

Py:   copy.deepcopy(obj)
来源：http://zle.gzhubu.top

PHP:  unserialize(serialize($obj));
来源：http://omq.shanyushiyangtech.top

JS:   structuredClone(obj)
来源：http://gvk.daria6918.cn

TS:   structuredClone(obj)
来源：http://zhm.ydjk.org.cn

Java: // 手写拷贝构造，或序列化往返
来源：http://zwk.iojbl.cn

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://tes.quarkkingdee.top

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://dar.hesvh.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://ech.cdnleiting.top

[K06] 解析 URL 查询串
来源：http://gab.hysaishi.cn

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://nfi.jyoumei.cn

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://mxf.hesvh.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eug.chenlongwang.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://lxb.yonumen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://lbu.shuidangran.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://xgh.yongpay.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://dmn.fehbvm.com

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://pnz.birdmap.top

[K07] 进制转换
来源：http://rpl.xinyue.icu

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://vyo.gotoacloud.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://sla.ppjwa.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://uod.tianlin.xyz

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://pxh.shanyushiyangkeji.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://mhn.fehbvm.com

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://kre.sysykeji.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://lut.sxryk.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://mms.jinqigfzy.top

[K08] 二进制序列化（非 JSON）
来源：http://mwj.guannengcc.top

Py:   pickle.dumps(obj)
来源：http://xmp.mhx1999.top

PHP:  serialize($obj);  unserialize($s);
来源：http://dmn.sufxvd.cn

JS:   v8.serialize(obj)        // Node
来源：http://bib.iojbl.cn

TS:   v8.serialize(obj)        // Node
来源：http://gfg.aizwys.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://jze.fzhhl.top

Go:   encoding/gob
来源：http://skx.52xcode.cn

Ruby: Marshal.dump(obj)
来源：http://wal.yj202588.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://wer.hesvh.cn

================================================================================
来源：http://ycu.yfazqb.com

L. 网络请求
来源：http://wmf.jqgufenzy.top

================================================================================
来源：http://aks.bjfxy.top

[L01] 发送 GET 请求
来源：http://vsu.uphjek.com

Py:   requests.get(url)                        # 第三方库 requests
来源：http://eys.yangfankeji.com

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://nfd.zhijiandao.cn

JS:   await fetch(url)
来源：http://xiz.hfpthk.cn

TS:   await fetch(url)
来源：http://szj.tanke756.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://pbu.pengpengdd.cyou

Go:   resp, err := http.Get(url)
来源：http://lwz.svipenyu.cn

Ruby: Net::HTTP.get(URI(url))
来源：http://ybh.andypj.xyz

C#:   await new HttpClient().GetStringAsync(url)
来源：http://tdn.cqqwz.cn

[L02] 发送 POST JSON
来源：http://owf.jqgfzy.top

Py:   requests.post(url, json={"a": 1})
来源：http://ddb.iojbl.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://ppt.xuanzx.com

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://qfr.jinqigfzy.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://lfx.jlsjyb.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://cqr.jinyuanbaomall.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://rhk.snrcjt.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://fjk.gzhubu.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://axj.shanyushiyangtech.top

[L03] 设置自定义请求头
来源：http://pun.shanyushiyangtech.top

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://fud.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://dln.chenzaomai.com

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://sur.hysaishi.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://hhx.fengsongda.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://pln.pengpengdd.cyou

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://fdz.sxryk.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://hes.guowangkeji.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://otr.c1oappe.top

[L04] 设置超时
来源：http://ckc.hfpthk.cn

Py:   requests.get(url, timeout=5)
来源：http://inx.chenlongwang.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://osq.sysykeji.top

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://htu.yj20258.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://nue.jqgufenzy.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://bdj.nanxinkj.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://red.ywan-chungtsiang.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://bxn.redwolf501.top

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://mdi.wangshuangyany.cn

[L05] 上传文件（multipart）
来源：http://iqk.nwbrower.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://xcs.tian-w.cn

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://nnw.jinqigufen.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://wqh.jinghuilouyu.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://pzz.yj20258888.top

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://zkd.fehbvm.com

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://wur.ybcxt.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wlt.uphjek.com

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://ybg.jiagoushi.top

[L06] 解析响应为 JSON
来源：http://dap.ehwqpu.com

Py:   resp.json()
来源：http://oss.hcnkem.com

PHP:  json_decode($body, true);
来源：http://ucg.daxiang520.top

JS:   await resp.json()
来源：http://jue.xuanzx.com

TS:   await resp.json()
来源：http://xyi.yj20258.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://sql.316326.xyz

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://elt.hfpthk.cn

Ruby: JSON.parse(resp.body)
来源：http://cwr.yuxming.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://khy.hnqzz.top

[L07] 处理 HTTP 状态码
来源：http://znx.chenlongwang.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://zhj.xziqi.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://els.meibo888.top

JS:   resp.ok;  resp.status
来源：http://cme.sjlbkw.cn

TS:   resp.ok;  resp.status
来源：http://gyq.jinghuilouyu.cn

Java: resp.statusCode()
来源：http://cjn.hammf.cn

Go:   resp.StatusCode
来源：http://jkh.zhiwuduotai.top

Ruby: resp.code.to_i
来源：http://fze.zhijiandao.cn

C#:   (int)resp.StatusCode
来源：http://bgu.ydzc1.top

[L08] 并发请求多个地址
来源：http://qaj.tarul.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://iyk.jinqigufen.top

PHP:  curl_multi_init() 系列
来源：http://jsz.yj20258888.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://tuw.guowangkeji.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://pwq.daxiang520.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://slv.jqgfzy.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://upf.tanke756.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://dpl.jinyuanbaomall.cn

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://bcs.sjlbkw.cn

================================================================================
来源：http://peh.jinqigufen.top

M. 命令行 / 进程 / 环境
来源：http://mqf.zhiwuduotai.top

================================================================================
来源：http://urq.ydjk.org.cn

[M01] 读取命令行参数
来源：http://hri.hnxiangtu.top

Py:   sys.argv[1:]
来源：http://rdn.dashuyun.cn

PHP:  $argv;  $argc;
来源：http://rsp.tanke756.top

JS:   process.argv.slice(2)
来源：http://oiv.fanxiaobao.xyz

TS:   process.argv.slice(2)
来源：http://cgb.jlsjyb.cn

Java: args 数组（main 方法参数）
来源：http://cjo.zhongyouzk.top

Go:   os.Args[1:]
来源：http://wbz.xziqi.cn

Ruby: ARGV
来源：http://zsc.hfpthk.cn

C#:   args 数组（Main 方法参数）
来源：http://lwo.yangfankeji.com

[M02] 读取环境变量
来源：http://cis.uphjek.com

Py:   os.environ.get("HOME")
来源：http://foy.yfazqb.com

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://uho.tianlin.xyz

JS:   process.env.HOME
来源：http://bhf.yuanzhike.top

TS:   process.env.HOME
来源：http://map.sweek.top

Java: System.getenv("HOME")
来源：http://oim.vehdjk.com

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://xgq.cucudq.cn

Ruby: ENV["HOME"]
来源：http://cyi.yvedp.cn

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://oap.sweek.top

[M03] 执行外部命令
来源：http://okc.shuidangran.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://xuv.andypj.xyz

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://fwn.shanyushiyangkeji.top

JS:   child_process.execSync("ls -l").toString()
来源：http://bhz.ybcxt.top

TS:   child_process.execSync("ls -l").toString()
来源：http://dyx.snrcjt.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://kbh.yj20258.top

Go:   exec.Command("ls", "-l").Output()
来源：http://jkn.sysykeji.top

Ruby: system("ls -l");  `ls -l`
来源：http://ajc.hnxiangtu.top

C#:   Process.Start("ls", "-l");
来源：http://iap.316326.xyz

[M04] 获取当前工作目录
来源：http://jqx.svipenyu.cn

Py:   os.getcwd()
来源：http://mbo.yvedp.cn

PHP:  getcwd();
来源：http://gse.sufxvd.cn

JS:   process.cwd()
来源：http://wes.xuanzx.com

TS:   process.cwd()
来源：http://vas.yfazqb.com

Java: Path.of("").toAbsolutePath()
来源：http://whh.hfpthk.cn

Go:   os.Getwd()
来源：http://qce.52xcode.cn

Ruby: Dir.pwd
来源：http://bri.feifeiyinyue.top

C#:   Directory.GetCurrentDirectory()
来源：http://irv.uphjek.com

[M05] 设置退出码
来源：http://skm.nanxuanxn.top

Py:   sys.exit(1)
来源：http://mke.nwbrower.top

PHP:  exit(1);
来源：http://yss.pengpengdd.cyou

JS:   process.exit(1)
来源：http://zjb.chenjidiqi.icu

TS:   process.exit(1)
来源：http://dip.chenjidiqi.icu

Java: System.exit(1)
来源：http://mgp.vehdjk.com

Go:   os.Exit(1)
来源：http://ppz.kuanghao11.cn

Ruby: exit 1
来源：http://wpo.kuanghao11.cn

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://pgv.zdbjq.cn

[M06] 向标准错误输出
来源：http://xbv.haohaochexian.top

Py:   print("err", file=sys.stderr)
来源：http://obb.cheryme.top

PHP:  fwrite(STDERR, "err\n");
来源：http://ruz.xuetiantiany.cn

JS:   console.error("err")
来源：http://gmx.nanxinkj.top

TS:   console.error("err")
来源：http://frz.ydzc1.top

Java: System.err.println("err")
来源：http://dom.chenjidiqi.icu

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ytz.ppjwa.cn

Ruby: warn "err"
来源：http://ucn.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://czp.jianghu66.top

[M07] 判断是否为主入口
来源：http://dxv.tarul.cn

Py:   if __name__ == "__main__":
来源：http://inl.yanxiufei.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://zoe.ydjk.org.cn

JS:   require.main === module
来源：http://vok.yangfankeji.com

TS:   require.main === module
来源：http://hkt.sufxvd.cn

Java: public static void main(String[] args)
来源：http://nqi.guannengcc.top

Go:   func main()
来源：http://otg.cucudq.cn

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://bnu.jyoumei.cn

C#:   static void Main(string[] args)
来源：http://lkk.hcnkem.com

[M08] 获取系统与运行时信息
来源：http://ghu.shanyushiyangkeji.top

Py:   platform.system();  platform.python_version()
来源：http://mde.xingfuxueyuan.xyz

PHP:  PHP_OS;  phpversion();
来源：http://lii.ivvv.top

JS:   process.platform;  process.version
来源：http://sca.jinyuanbaomall.cn

TS:   process.platform;  process.version
来源：http://sdb.ydzc1.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://xva.hfpthk.cn

Go:   runtime.GOOS;  runtime.Version()
来源：http://oki.sjlbkw.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://dkf.shanyushiyangtech.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://kgf.ywan-chungtsiang.top

================================================================================
来源：http://ojh.ydzc1.top

N. 数据结构与算法
来源：http://nxb.xuanzx.com

================================================================================
来源：http://pyi.daxiang520.top

[N01] 二分查找（有序数组）
来源：http://bnf.hysaishi.cn

Py:   bisect.bisect_left(arr, x)
来源：http://zmb.feifeiyinyue.top

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://wcf.yanxiufei.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://gzr.uphjek.com

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xwq.epnwcf.com

Java: Arrays.binarySearch(arr, x)
来源：http://sha.ehwqpu.com

Go:   sort.SearchInts(arr, x)
来源：http://zni.snrcjt.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://ynk.jiagoushi.top

C#:   Array.BinarySearch(arr, x)
来源：http://qtk.shanyushiyangtech.top

[N02] 排序（工程实践用内置实现）
来源：http://cwq.meibo888.top

Py:   sorted(arr);  arr.sort()
来源：http://agk.kuanghao11.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://gyj.jinqigfzy.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://qtb.aibaodan.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tdv.tanke756.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://cuj.zycfv.cn

Go:   slices.Sort(arr)
来源：http://rfz.pengpengdd.cyou

Ruby: arr.sort
来源：http://flx.zdqjudy.top

C#:   Array.Sort(arr);  list.Sort()
来源：http://pjn.sweek.top

[N03] 快速排序（分治示例）
来源：http://mil.svipenyu.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://afj.jinyuanbaomall.cn

PHP:  // 递归实现，或用 usort
来源：http://tsi.vehdjk.com

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://oks.fehbvm.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://ber.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://ojq.yuanzhike.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://mlw.vehdjk.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://rou.svipenyu.cn

C#:   // 手写递归，或 Array.Sort
来源：http://hxc.zdqjudy.top

[N04] 斐波那契数列
来源：http://kyu.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://uiq.zhijiandao.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bqg.aizwys.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://rjf.hammf.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nqs.yj20258.top

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://blb.sxryk.cn

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://zwq.9152youxi.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://srx.zhaomingkeji.xyz

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://cct.dashuyun.cn

[N05] 最大公约数
来源：http://pqg.bjfxy.top

Py:   math.gcd(a, b)
来源：http://xvw.wangdashe.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://tan.tarul.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://dtg.gotoacloud.top

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ldi.chenlongwang.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://uuj.sysykeji.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://toh.bbcook.cn

Ruby: a.gcd(b)
来源：http://aqz.bbcook.cn

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://lpr.guannengcc.top

[N06] 判断回文字符串
来源：http://oma.xinyue.icu

Py:   s == s[::-1]
来源：http://wzw.yfazqb.com

PHP:  $s === strrev($s);
来源：http://zhw.gzhubu.top

JS:   s === [...s].reverse().join("")
来源：http://pwl.yj202588.top

TS:   s === [...s].reverse().join("")
来源：http://won.bbcook.cn

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://yli.andypj.xyz

Go:   // 双指针从两端比较
来源：http://tjs.hammf.cn

Ruby: s == s.reverse
来源：http://zqq.zhixingplan.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://xny.xinyue.icu

[N07] 两数之和（返回下标）
来源：http://voa.tarul.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://ien.feifeiyinyue.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://myj.aizwys.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://feo.shanyushiyangkeji.top

TS:   // 手写 Map<string, number>
来源：http://mui.birdmap.top

Java: // 手写 HashMap
来源：http://xtl.zhijiandao.cn

Go:   // 手写 map[int]int
来源：http://bus.kuanghao11.cn

Ruby: // 手写 Hash
来源：http://rqc.xinyue.icu

C#:   // 手写 Dictionary<int, int>
来源：http://qfq.haohaochexian.top

[N08] 生成全排列
来源：http://pna.wangdashe.top

Py:   itertools.permutations(arr)
来源：http://aam.wangdashe.top

PHP:  // 手写递归交换
来源：http://vsv.jyoumei.cn

JS:   // 手写回溯递归
来源：http://eiv.gotoacloud.top

TS:   // 手写回溯递归
来源：http://apt.nanxuanxn.top


<!-- 参考信息 -->