代发 wailian999

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://vcx.fzhhl.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://vxs.52xcode.cn

JS:   JSON.stringify(obj)
来源：http://wjm.jinqigufen.top

TS:   JSON.stringify(obj)
来源：http://eyv.zhengqikj.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://jcx.yj202588.top

Go:   json.Marshal(obj)
来源：http://vnj.wangdashe.top

Ruby: obj.to_json                                     // require "json"
来源：http://ixh.aibaodan.cn

C#:   JsonSerializer.Serialize(obj)
来源：http://iax.pengpengdd.cyou

[K02] JSON 字符串转对象
来源：http://vsn.ywan-chungtsiang.top

Py:   json.loads(s)
来源：http://guh.zhaomingkeji.xyz

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://ftm.zdbjq.cn

JS:   JSON.parse(s)
来源：http://mev.kuanghao11.cn

TS:   JSON.parse(s)
来源：http://eju.yj20258888.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://wrv.fehbvm.com

Go:   json.Unmarshal(data, &v)
来源：http://goe.bbcook.cn

Ruby: JSON.parse(s)
来源：http://kme.chenjidiqi.icu

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://zzi.ydzc1.top

[K03] JSON 美化输出（带缩进）
来源：http://xnd.hongshengwenyu.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://dwk.andypj.xyz

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://zdy.zhiwuduotai.top

JS:   JSON.stringify(obj, null, 2)
来源：http://deu.cdnleiting.top

TS:   JSON.stringify(obj, null, 2)
来源：http://imp.jqgufenzy.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://hlz.yangfankeji.com

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://nbg.uphjek.com

Ruby: JSON.pretty_generate(obj)
来源：http://hmp.ppjwa.cn

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://eth.jianghu66.top

[K04] 读取 JSON 文件
来源：http://jci.havefunace.top

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://lse.guowangkeji.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://oys.vehdjk.com

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://kwm.nwbrower.top

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://zcb.aibaodan.cn

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://yde.sjlbkw.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://gph.ivvv.top

Ruby: JSON.parse(File.read("a.json"))
来源：http://mra.cdnleiting.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://ihi.yfazqb.com

[K05] 深拷贝对象
来源：http://owq.hongshengwenyu.top

Py:   copy.deepcopy(obj)
来源：http://wlb.smart0.xyz

PHP:  unserialize(serialize($obj));
来源：http://psz.zhiwuduotai.top

JS:   structuredClone(obj)
来源：http://inv.tian-w.cn

TS:   structuredClone(obj)
来源：http://fhs.yangfankeji.com

Java: // 手写拷贝构造，或序列化往返
来源：http://dge.pycfn.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://fxu.wangshuangyany.cn

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://ckk.9152youxi.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://cdq.yuxming.cn

[K06] 解析 URL 查询串
来源：http://dwr.cdnleiting.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://qdf.vehdjk.com

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://pfp.9152youxi.cn

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://mvj.xylfe.cn

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://uew.xuetiantiany.cn

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://ysu.xziqi.cn

Go:   url.ParseQuery("a=1&b=2")
来源：http://mds.jianghu66.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://mfe.xylfe.cn

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://nhr.ppjwa.cn

[K07] 进制转换
来源：http://mir.sufxvd.cn

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://dkd.shanyushiyangtech.top

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://gob.tarul.cn

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://xxi.hnqzz.top

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://anb.zhixingplan.top

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://wyv.xylfe.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://jcc.feifeiyinyue.top

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://nmn.tarul.cn

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://uyp.zhijiandao.cn

[K08] 二进制序列化（非 JSON）
来源：http://vsa.meibo888.top

Py:   pickle.dumps(obj)
来源：http://ree.hesvh.cn

PHP:  serialize($obj);  unserialize($s);
来源：http://pkn.uphjek.com

JS:   v8.serialize(obj)        // Node
来源：http://wjq.fehbvm.com

TS:   v8.serialize(obj)        // Node
来源：http://pfx.zhijiandao.cn

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://lso.redwolf501.top

Go:   encoding/gob
来源：http://uyp.hcnkem.com

Ruby: Marshal.dump(obj)
来源：http://zej.jqgfzy.top

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://kyg.shzxlz.cn

================================================================================
来源：http://mgz.vqdsnc.cn

L. 网络请求
来源：http://jqn.daria6918.cn

================================================================================
来源：http://url.bbcook.cn

[L01] 发送 GET 请求
来源：http://qnh.nanxinkj.top

Py:   requests.get(url)                        # 第三方库 requests
来源：http://omb.jinqigufen.top

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://snj.shangyingyoupin.top

JS:   await fetch(url)
来源：http://zha.snrcjt.cn

TS:   await fetch(url)
来源：http://unn.fktsv.cn

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://obb.jiagoushi.top

Go:   resp, err := http.Get(url)
来源：http://rcc.ehwqpu.com

Ruby: Net::HTTP.get(URI(url))
来源：http://rri.quarkkingdee.top

C#:   await new HttpClient().GetStringAsync(url)
来源：http://zqa.jinqigfzy.top

[L02] 发送 POST JSON
来源：http://ert.sxryk.cn

Py:   requests.post(url, json={"a": 1})
来源：http://bdt.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://slo.ydjk.org.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://cal.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://dio.zhaomingkeji.xyz

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://hdd.cdnleiting.top

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://wjb.fengsongda.top

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://bwu.zhiwuduotai.top

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://ght.xylfe.cn

[L03] 设置自定义请求头
来源：http://ial.ppjwa.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://clv.fanxiaobao.xyz

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://yrm.yongpay.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://egf.52xcode.cn

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://uey.dashuyun.cn

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://mwe.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://xpp.tarul.cn

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://puy.guannengcc.top

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://tqf.snrcjt.cn

[L04] 设置超时
来源：http://myg.jinyuanbaomall.cn

Py:   requests.get(url, timeout=5)
来源：http://xpp.cqqwz.cn

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://tzp.uphjek.com

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://afj.shanyushiyangtech.top

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zrg.haohaochexian.top

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://kxz.daria6918.cn

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://cml.daxiang520.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://mmf.0kj1m.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://aha.pycfn.com

[L05] 上传文件（multipart）
来源：http://nom.guannengcc.top

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://hnv.sweek.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://kqq.sysykeji.top

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://xhc.sufxvd.cn

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://etp.sxryk.cn

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://wcb.yj202588.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://ghx.redwolf501.top

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://egn.quarkkingdee.top

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://hmu.xziqi.cn

[L06] 解析响应为 JSON
来源：http://ciw.shuidangran.top

Py:   resp.json()
来源：http://xho.jqgufenzy.top

PHP:  json_decode($body, true);
来源：http://kpc.xinyue.icu

JS:   await resp.json()
来源：http://cmm.cdnleiting.top

TS:   await resp.json()
来源：http://jyd.chenjidiqi.icu

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://cta.cashguo.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://gmt.guannengcc.top

Ruby: JSON.parse(resp.body)
来源：http://xew.gogol.net.cn

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://qub.9152youxi.cn

[L07] 处理 HTTP 状态码
来源：http://wul.dashuyun.cn

Py:   resp.status_code;  resp.raise_for_status()
来源：http://wpg.sxryk.cn

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://ark.hongshengwenyu.top

JS:   resp.ok;  resp.status
来源：http://tdt.hnxiangtu.top

TS:   resp.ok;  resp.status
来源：http://mdy.havefunace.top

Java: resp.statusCode()
来源：http://lai.shuidangran.top

Go:   resp.StatusCode
来源：http://has.guowangkeji.top

Ruby: resp.code.to_i
来源：http://huz.hysaishi.cn

C#:   (int)resp.StatusCode
来源：http://ety.fanxiaobao.xyz

[L08] 并发请求多个地址
来源：http://hgd.zhengqikj.top

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://vol.xylfe.cn

PHP:  curl_multi_init() 系列
来源：http://qfz.xinyue.icu

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://vkx.zhengqikj.top

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://obg.yueranfly.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ecg.fengsongda.top

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://xqv.sysykeji.top

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://kuw.mhx1999.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://cfu.zdbjq.cn

================================================================================
来源：http://exa.iojbl.cn

M. 命令行 / 进程 / 环境
来源：http://nfw.fzhhl.top

================================================================================
来源：http://php.daxiang520.top

[M01] 读取命令行参数
来源：http://rbs.shanyushiyangtech.top

Py:   sys.argv[1:]
来源：http://wrt.yanxiufei.cn

PHP:  $argv;  $argc;
来源：http://pmy.gzhubu.top

JS:   process.argv.slice(2)
来源：http://cni.chenzaomai.com

TS:   process.argv.slice(2)
来源：http://roz.shangyingyoupin.top

Java: args 数组（main 方法参数）
来源：http://xdp.cqqwz.cn

Go:   os.Args[1:]
来源：http://buf.fzhhl.top

Ruby: ARGV
来源：http://mut.guannengcc.top

C#:   args 数组（Main 方法参数）
来源：http://ltx.hnqzz.top

[M02] 读取环境变量
来源：http://tqs.xuetiantiany.cn

Py:   os.environ.get("HOME")
来源：http://vtv.ppjwa.cn

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://rjz.sufxvd.cn

JS:   process.env.HOME
来源：http://opq.gaohongyu789.top

TS:   process.env.HOME
来源：http://nyh.fengsongda.top

Java: System.getenv("HOME")
来源：http://wni.guannengcc.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://nad.vqdsnc.cn

Ruby: ENV["HOME"]
来源：http://xco.chenjidiqi.icu

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://yec.yj20258.top

[M03] 执行外部命令
来源：http://vfn.jqgfzy.top

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://lka.hywenlv.cn

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://ikg.aizwys.cn

JS:   child_process.execSync("ls -l").toString()
来源：http://gwu.andypj.xyz

TS:   child_process.execSync("ls -l").toString()
来源：http://rci.ppjwa.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://xtb.jqgufenzy.top

Go:   exec.Command("ls", "-l").Output()
来源：http://bkb.sxryk.cn

Ruby: system("ls -l");  `ls -l`
来源：http://iea.yanxiufei.cn

C#:   Process.Start("ls", "-l");
来源：http://tkz.jqgfzy.top

[M04] 获取当前工作目录
来源：http://jvw.jinqigfzy.top

Py:   os.getcwd()
来源：http://igk.jinqigufen.top

PHP:  getcwd();
来源：http://qdi.yonumen.top

JS:   process.cwd()
来源：http://zbg.svipenyu.cn

TS:   process.cwd()
来源：http://qqv.jinyuanbaomall.cn

Java: Path.of("").toAbsolutePath()
来源：http://lbx.tanke756.top

Go:   os.Getwd()
来源：http://oui.shzxlz.cn

Ruby: Dir.pwd
来源：http://opy.yj20258.top

C#:   Directory.GetCurrentDirectory()
来源：http://kyq.ybcxt.top

[M05] 设置退出码
来源：http://ptx.hfpthk.cn

Py:   sys.exit(1)
来源：http://crz.cheryme.top

PHP:  exit(1);
来源：http://ild.kuanghao11.cn

JS:   process.exit(1)
来源：http://zff.ppjwa.cn

TS:   process.exit(1)
来源：http://rdg.zhongyouzk.top

Java: System.exit(1)
来源：http://ycc.uphjek.com

Go:   os.Exit(1)
来源：http://szg.ydzc1.top

Ruby: exit 1
来源：http://ino.yuanzhike.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://vgc.xuetiantiany.cn

[M06] 向标准错误输出
来源：http://xws.snrcjt.cn

Py:   print("err", file=sys.stderr)
来源：http://aqf.hammf.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://fcu.xylfe.cn

JS:   console.error("err")
来源：http://ivq.jianghu66.top

TS:   console.error("err")
来源：http://gbs.jiagoushi.top

Java: System.err.println("err")
来源：http://vng.tanke756.top

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://ufn.bjfxy.top

Ruby: warn "err"
来源：http://gwe.vehdjk.com

C#:   Console.Error.WriteLine("err")
来源：http://sgt.pycfn.com

[M07] 判断是否为主入口
来源：http://tgb.vqdsnc.cn

Py:   if __name__ == "__main__":
来源：http://ksd.c1oappe.top

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://uip.zhongyouzk.top

JS:   require.main === module
来源：http://ral.tianlin.xyz

TS:   require.main === module
来源：http://ild.ywan-chungtsiang.top

Java: public static void main(String[] args)
来源：http://nae.chenzaomai.com

Go:   func main()
来源：http://peg.cdnleiting.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ykz.havefunace.top

C#:   static void Main(string[] args)
来源：http://qdc.jinyuanbaomall.cn

[M08] 获取系统与运行时信息
来源：http://fvt.bbcook.cn

Py:   platform.system();  platform.python_version()
来源：http://dae.xziqi.cn

PHP:  PHP_OS;  phpversion();
来源：http://yun.shzxlz.cn

JS:   process.platform;  process.version
来源：http://qgd.snrcjt.cn

TS:   process.platform;  process.version
来源：http://uce.cdnleiting.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://kfq.jqgfzy.top

Go:   runtime.GOOS;  runtime.Version()
来源：http://lym.jinyuanbaomall.cn

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://kmn.kuanghao11.cn

C#:   Environment.OSVersion;  Environment.Version
来源：http://xgz.bbcook.cn

================================================================================
来源：http://bsr.yonumen.top

N. 数据结构与算法
来源：http://eps.jlsjyb.cn

================================================================================
来源：http://gwy.fehbvm.com

[N01] 二分查找（有序数组）
来源：http://wkf.fanxiaobao.xyz

Py:   bisect.bisect_left(arr, x)
来源：http://kbl.sjlbkw.cn

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://vvy.cucudq.cn

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://kym.cqqwz.cn

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://xqu.xinyue.icu

Java: Arrays.binarySearch(arr, x)
来源：http://vxh.gzhubu.top

Go:   sort.SearchInts(arr, x)
来源：http://nlf.shangyingyoupin.top

Ruby: arr.bsearch { |e| e >= x }
来源：http://rzs.haohaochexian.top

C#:   Array.BinarySearch(arr, x)
来源：http://qtx.hongshengwenyu.top

[N02] 排序（工程实践用内置实现）
来源：http://mvi.yongpay.top

Py:   sorted(arr);  arr.sort()
来源：http://kec.zhoulong.xyz

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://odp.yongpay.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://brm.jqgufenzy.top

TS:   [...arr].sort((a, b) => a - b)
来源：http://mgc.shangyingyoupin.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://qjf.zhaomingkeji.xyz

Go:   slices.Sort(arr)
来源：http://oqz.guannengcc.top

Ruby: arr.sort
来源：http://sjs.yuxming.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://isk.smart0.xyz

[N03] 快速排序（分治示例）
来源：http://ycj.cqqwz.cn

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://adm.hammf.cn

PHP:  // 递归实现，或用 usort
来源：http://ppb.bjfxy.top

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://yvp.pycfn.com

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://iqi.cashguo.top

Java: // 手写递归，或直接用 Arrays.sort
来源：http://bkp.chenlongwang.top

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://ksq.pycfn.com

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://ukt.shanyushiyangtech.top

C#:   // 手写递归，或 Array.Sort
来源：http://vxj.aibaodan.cn

[N04] 斐波那契数列
来源：http://eqd.mhx1999.top

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://hfy.tian-w.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://bmo.vqdsnc.cn

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://nmx.fzhhl.top

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://sxp.fktsv.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://spv.ehwqpu.com

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://lcg.hongshengwenyu.top

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://tft.52xcode.cn

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://ups.feifeiyinyue.top

[N05] 最大公约数
来源：http://xob.guannengcc.top

Py:   math.gcd(a, b)
来源：http://ozj.316326.xyz

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://vgd.dashuyun.cn

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://ong.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://imk.pengpengdd.cyou

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://byb.cashguo.top

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://qzj.dianchejie.cn

Ruby: a.gcd(b)
来源：http://uds.guannengcc.top

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://uzo.9152youxi.cn

[N06] 判断回文字符串
来源：http://twu.jqgufenzy.top

Py:   s == s[::-1]
来源：http://llx.hesvh.cn

PHP:  $s === strrev($s);
来源：http://gac.feifeiyinyue.top

JS:   s === [...s].reverse().join("")
来源：http://yzp.shanyushiyangkeji.top

TS:   s === [...s].reverse().join("")
来源：http://ekm.feifeiyinyue.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://bkb.tarul.cn

Go:   // 双指针从两端比较
来源：http://wpn.shanyushiyangkeji.top

Ruby: s == s.reverse
来源：http://wda.0kj1m.cn

C#:   s == new string(s.Reverse().ToArray())
来源：http://ogf.316326.xyz

[N07] 两数之和（返回下标）
来源：http://ubz.wangshuangyany.cn

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://qll.quarkkingdee.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://uoj.yanxiufei.cn

JS:   // 手写 Map：map.set(v, i)
来源：http://dia.fanxiaobao.xyz

TS:   // 手写 Map<string, number>
来源：http://rti.sufxvd.cn

Java: // 手写 HashMap
来源：http://rbu.chenjidiqi.icu

Go:   // 手写 map[int]int
来源：http://zfx.xingfuxueyuan.xyz

Ruby: // 手写 Hash
来源：http://mri.hammf.cn

C#:   // 手写 Dictionary<int, int>
来源：http://sjq.ctjpmb.com

[N08] 生成全排列
来源：http://clv.jinyuanbaomall.cn

Py:   itertools.permutations(arr)
来源：http://chp.hesvh.cn

PHP:  // 手写递归交换
来源：http://gqo.svipenyu.cn

JS:   // 手写回溯递归
来源：http://osh.mhx1999.top

TS:   // 手写回溯递归
来源：http://auh.sjlbkw.cn

Java: // 手写回溯递归
来源：http://nul.zhixingplan.top

Go:   // 手写回溯递归
来源：http://pzk.zycfv.cn

Ruby: arr.permutation.to_a
来源：http://pgo.yj202588.top

C#:   // 手写回溯递归
来源：http://leq.jinghuilouyu.cn

[N09] 栈与队列
来源：http://ueu.fzhhl.top

Py:   stack.append(x) / stack.pop()；deque.popleft() 作队列
来源：http://lfy.quarkkingdee.top

PHP:  array_push/array_pop 作栈；array_shift 作队列
来源：http://avc.cucudq.cn

JS:   arr.push(x) / arr.pop() 作栈；arr.push / arr.shift 作队列
来源：http://tvw.quarkkingdee.top


<!-- 参考信息 -->