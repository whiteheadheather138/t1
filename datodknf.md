代发 wailian999

Py:   date.today();  date.today().replace(day=1)
来源：http://ohx.guowangkeji.top

PHP:  new DateTime("today");  new DateTime("first day of this month");
来源：http://stj.ctjpmb.com

JS:   new Date().setHours(0, 0, 0, 0);  new Date(y, m, 1)
来源：http://nyz.hywenlv.cn

TS:   new Date().setHours(0, 0, 0, 0)
来源：http://sna.nanxinkj.top

Java: LocalDate.now();  LocalDate.now().withDayOfMonth(1)
来源：http://hky.hongshengwenyu.top

Go:   now := time.Now();  time.Date(now.Year(), now.Month(), 1, 0, 0, 0, 0, now.Location())
来源：http://kig.sxryk.cn

Ruby: Date.today;  Date.today.next_month - Date.today.day   # 本月最后一天思路
来源：http://swj.hywenlv.cn

C#:   DateTime.Today;  new DateTime(now.Year, now.Month, 1)
来源：http://xxw.jinyuanbaomall.cn

================================================================================
来源：http://mns.xinyue.icu

K. JSON 与序列化
来源：http://qmc.jiagoushi.top

================================================================================
来源：http://qcr.shuidangran.top

[K01] 对象转 JSON 字符串
来源：http://piv.xuetiantiany.cn

Py:   json.dumps(obj, ensure_ascii=False)
来源：http://axj.shanyushiyangkeji.top

PHP:  json_encode($obj, JSON_UNESCAPED_UNICODE);
来源：http://dzs.iojbl.cn

JS:   JSON.stringify(obj)
来源：http://zqe.wangshuangyany.cn

TS:   JSON.stringify(obj)
来源：http://iht.nanxuanxn.top

Java: new ObjectMapper().writeValueAsString(obj)      // Jackson
来源：http://lyn.jinqigfzy.top

Go:   json.Marshal(obj)
来源：http://dsl.fehbvm.com

Ruby: obj.to_json                                     // require "json"
来源：http://awd.haohaochexian.top

C#:   JsonSerializer.Serialize(obj)
来源：http://aii.shanyushiyangtech.top

[K02] JSON 字符串转对象
来源：http://jjz.fanxiaobao.xyz

Py:   json.loads(s)
来源：http://pjt.fktsv.cn

PHP:  json_decode($s, true);                          // true 得关联数组
来源：http://zzo.nanxinkj.top

JS:   JSON.parse(s)
来源：http://fkx.feifeiyinyue.top

TS:   JSON.parse(s)
来源：http://nzz.ywan-chungtsiang.top

Java: new ObjectMapper().readValue(s, Map.class)
来源：http://irq.jlsjyb.cn

Go:   json.Unmarshal(data, &v)
来源：http://hpo.xuanzx.com

Ruby: JSON.parse(s)
来源：http://mnm.sjlbkw.cn

C#:   JsonSerializer.Deserialize<T>(s)
来源：http://wyt.sjlbkw.cn

[K03] JSON 美化输出（带缩进）
来源：http://sne.chenlongwang.top

Py:   json.dumps(obj, indent=2, ensure_ascii=False)
来源：http://uvd.bbcook.cn

PHP:  json_encode($obj, JSON_PRETTY_PRINT | JSON_UNESCAPED_UNICODE);
来源：http://ioc.xylfe.cn

JS:   JSON.stringify(obj, null, 2)
来源：http://njm.meibo888.top

TS:   JSON.stringify(obj, null, 2)
来源：http://hbn.fzhhl.top

Java: mapper.writerWithDefaultPrettyPrinter().writeValueAsString(obj)
来源：http://whq.yanxiufei.cn

Go:   json.MarshalIndent(obj, "", "  ")
来源：http://ecr.xuetiantiany.cn

Ruby: JSON.pretty_generate(obj)
来源：http://zui.feifeiyinyue.top

C#:   JsonSerializer.Serialize(obj, new JsonSerializerOptions { WriteIndented = true })
来源：http://vgr.hnqzz.top

[K04] 读取 JSON 文件
来源：http://dka.dashuyun.cn

Py:   json.load(open("a.json", encoding="utf-8"))
来源：http://tpj.cashguo.top

PHP:  json_decode(file_get_contents("a.json"), true);
来源：http://uvt.guannengcc.top

JS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://yyj.bbcook.cn

TS:   JSON.parse(fs.readFileSync("a.json", "utf8"))
来源：http://jzc.fzhhl.top

Java: mapper.readValue(new File("a.json"), Map.class)
来源：http://njd.tarul.cn

Go:   data, _ := os.ReadFile("a.json");  json.Unmarshal(data, &v)
来源：http://vqj.yvedp.cn

Ruby: JSON.parse(File.read("a.json"))
来源：http://gti.redwolf501.top

C#:   JsonSerializer.Deserialize<T>(File.ReadAllText("a.json"))
来源：http://tuj.haohaochexian.top

[K05] 深拷贝对象
来源：http://vga.wangshuangyany.cn

Py:   copy.deepcopy(obj)
来源：http://bwq.zycfv.cn

PHP:  unserialize(serialize($obj));
来源：http://yqd.zhiwuduotai.top

JS:   structuredClone(obj)
来源：http://pgz.chenjidiqi.icu

TS:   structuredClone(obj)
来源：http://qpp.gzhubu.top

Java: // 手写拷贝构造，或序列化往返
来源：http://ydg.xuanzx.com

Go:   // 结构体值赋值即复制（注意指针/切片字段）
来源：http://eho.316326.xyz

Ruby: Marshal.load(Marshal.dump(obj))
来源：http://wlq.jlsjyb.cn

C#:   // 序列化往返，或自定义 Clone
来源：http://vyp.yongpay.top

[K06] 解析 URL 查询串
来源：http://ccq.yuanzhike.top

Py:   parse_qs("a=1&b=2");  urlencode({"a": 1})
来源：http://saf.nwbrower.top

PHP:  parse_str("a=1&b=2", $out);  http_build_query(["a" => 1]);
来源：http://ahk.shangyingyoupin.top

JS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://eiz.daxiang520.top

TS:   new URLSearchParams("a=1&b=2").get("a")
来源：http://otj.jinqigufen.top

Java: // 手动 split & 与 =，或 UriComponentsBuilder
来源：http://epc.jinqigufen.top

Go:   url.ParseQuery("a=1&b=2")
来源：http://tjz.yj20258.top

Ruby: URI.decode_www_form("a=1&b=2")
来源：http://xcl.hnxiangtu.top

C#:   HttpUtility.ParseQueryString("a=1&b=2")
来源：http://baq.jqgufenzy.top

[K07] 进制转换
来源：http://vdl.chenzaomai.com

Py:   bin(10);  hex(255);  int("ff", 16)
来源：http://udd.bbcook.cn

PHP:  decbin(10);  dechex(255);  hexdec("ff");
来源：http://pvm.jiagoushi.top

JS:   (10).toString(2);  (255).toString(16);  parseInt("ff", 16)
来源：http://lrs.wangshuangyany.cn

TS:   (10).toString(2);  parseInt("ff", 16)
来源：http://tcg.tian-w.cn

Java: Integer.toBinaryString(10);  Integer.toHexString(255);  Integer.parseInt("ff", 16)
来源：http://chk.bbcook.cn

Go:   strconv.FormatInt(10, 2);  strconv.ParseInt("ff", 16, 64)
来源：http://rfx.0kj1m.cn

Ruby: 10.to_s(2);  255.to_s(16);  "ff".to_i(16)
来源：http://grw.yongpay.top

C#:   Convert.ToString(10, 2);  Convert.ToString(255, 16);  Convert.ToInt32("ff", 16)
来源：http://psz.cashguo.top

[K08] 二进制序列化（非 JSON）
来源：http://ygu.sufxvd.cn

Py:   pickle.dumps(obj)
来源：http://avq.smart0.xyz

PHP:  serialize($obj);  unserialize($s);
来源：http://ecd.316326.xyz

JS:   v8.serialize(obj)        // Node
来源：http://wci.yfazqb.com

TS:   v8.serialize(obj)        // Node
来源：http://rti.quarkkingdee.top

Java: // 用 Kryo / Protobuf；Java 原生序列化已不推荐
来源：http://zsj.zhixingplan.top

Go:   encoding/gob
来源：http://afp.sufxvd.cn

Ruby: Marshal.dump(obj)
来源：http://akh.sufxvd.cn

C#:   // BinaryFormatter 已弃用，改用 MessagePack / System.Text.Json
来源：http://bjm.hnxiangtu.top

================================================================================
来源：http://ojv.xuetiantiany.cn

L. 网络请求
来源：http://fqb.fktsv.cn

================================================================================
来源：http://zhi.feifeiyinyue.top

[L01] 发送 GET 请求
来源：http://fgl.cucudq.cn

Py:   requests.get(url)                        # 第三方库 requests
来源：http://qcb.xylfe.cn

PHP:  file_get_contents($url);                 // 简单场景；复杂用 curl
来源：http://atb.ehwqpu.com

JS:   await fetch(url)
来源：http://iar.snrcjt.cn

TS:   await fetch(url)
来源：http://ath.gaohongyu789.top

Java: HttpClient.newHttpClient().send(HttpRequest.newBuilder(URI.create(url)).build(), BodyHandlers.ofString())
来源：http://wvr.andypj.xyz

Go:   resp, err := http.Get(url)
来源：http://kjg.yj202588.top

Ruby: Net::HTTP.get(URI(url))
来源：http://qaz.zhijiandao.cn

C#:   await new HttpClient().GetStringAsync(url)
来源：http://ouu.xuetiantiany.cn

[L02] 发送 POST JSON
来源：http://aqa.gogol.net.cn

Py:   requests.post(url, json={"a": 1})
来源：http://tkz.ehwqpu.com

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, json_encode(["a" => 1]));
来源：http://gqb.yuxming.cn

JS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://rau.jiagoushi.top

TS:   fetch(url, { method: "POST", headers: { "Content-Type": "application/json" }, body: JSON.stringify({ a: 1 }) })
来源：http://jhm.ppjwa.cn

Java: HttpRequest.newBuilder(uri).header("Content-Type", "application/json").POST(BodyPublishers.ofString(body)).build()
来源：http://irh.dashuyun.cn

Go:   http.Post(url, "application/json", strings.NewReader(`{"a":1}`))
来源：http://pck.sxryk.cn

Ruby: Net::HTTP.post(URI(url), '{"a":1}', "Content-Type" => "application/json")
来源：http://gyf.hammf.cn

C#:   await client.PostAsync(url, new StringContent(json, Encoding.UTF8, "application/json"))
来源：http://bot.zhiwuduotai.top

[L03] 设置自定义请求头
来源：http://jdu.zdbjq.cn

Py:   requests.get(url, headers={"X-Token": "abc"})
来源：http://zrj.ywan-chungtsiang.top

PHP:  curl_setopt($ch, CURLOPT_HTTPHEADER, ["X-Token: abc"]);
来源：http://fdl.shangyingyoupin.top

JS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://tmp.c1oappe.top

TS:   fetch(url, { headers: { "X-Token": "abc" } })
来源：http://was.fzhhl.top

Java: HttpRequest.newBuilder(uri).header("X-Token", "abc").build()
来源：http://hpq.jiagoushi.top

Go:   req, _ := http.NewRequest("GET", url, nil);  req.Header.Set("X-Token", "abc")
来源：http://rft.ivvv.top

Ruby: req = Net::HTTP::Get.new(uri);  req["X-Token"] = "abc"
来源：http://cdq.fehbvm.com

C#:   var req = new HttpRequestMessage(HttpMethod.Get, url);  req.Headers.Add("X-Token", "abc")
来源：http://kin.vqdsnc.cn

[L04] 设置超时
来源：http://tak.haohaochexian.top

Py:   requests.get(url, timeout=5)
来源：http://cvl.ivvv.top

PHP:  curl_setopt($ch, CURLOPT_TIMEOUT, 5);
来源：http://ozd.dashuyun.cn

JS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://cpo.zhaomingkeji.xyz

TS:   fetch(url, { signal: AbortSignal.timeout(5000) })
来源：http://zmo.cucudq.cn

Java: HttpClient.newBuilder().connectTimeout(Duration.ofSeconds(5)).build()
来源：http://cpc.shuidangran.top

Go:   client := &http.Client{Timeout: 5 * time.Second}
来源：http://aof.shanyushiyangtech.top

Ruby: Net::HTTP.start(uri.host, uri.port, open_timeout: 5, read_timeout: 5)
来源：http://fnh.yanxiufei.cn

C#:   client.Timeout = TimeSpan.FromSeconds(5);
来源：http://rti.zycfv.cn

[L05] 上传文件（multipart）
来源：http://yww.0kj1m.cn

Py:   requests.post(url, files={"f": open("a.txt", "rb")})
来源：http://ooc.gzhubu.top

PHP:  curl_setopt($ch, CURLOPT_POSTFIELDS, ["f" => new CURLFile("a.txt")]);
来源：http://phs.dashuyun.cn

JS:   const fd = new FormData();  fd.append("f", blob);  fetch(url, { method: "POST", body: fd })
来源：http://rrf.zhoulong.xyz

TS:   const fd = new FormData();  fetch(url, { method: "POST", body: fd })
来源：http://urx.smart0.xyz

Java: // 用 BodyPublishers.ofFile 或手写 multipart
来源：http://szn.jinqigfzy.top

Go:   mime/multipart.NewWriter 写入字段与文件
来源：http://bds.hywenlv.cn

Ruby: req.set_form([["f", File.open("a.txt")]])
来源：http://wnb.aizwys.cn

C#:   var form = new MultipartFormDataContent();  form.Add(new StreamContent(stream), "f", "a.txt");
来源：http://dsx.ctjpmb.com

[L06] 解析响应为 JSON
来源：http://qgm.jianghu66.top

Py:   resp.json()
来源：http://ece.yangfankeji.com

PHP:  json_decode($body, true);
来源：http://eyj.nanxuanxn.top

JS:   await resp.json()
来源：http://pvi.sxryk.cn

TS:   await resp.json()
来源：http://ndv.zhengqikj.top

Java: new ObjectMapper().readValue(resp.body(), Map.class)
来源：http://efp.hnqzz.top

Go:   json.NewDecoder(resp.Body).Decode(&v)
来源：http://bca.guannengcc.top

Ruby: JSON.parse(resp.body)
来源：http://crd.jqgfzy.top

C#:   await resp.Content.ReadFromJsonAsync<T>()
来源：http://xps.xingfuxueyuan.xyz

[L07] 处理 HTTP 状态码
来源：http://ckh.sweek.top

Py:   resp.status_code;  resp.raise_for_status()
来源：http://uwn.nanxinkj.top

PHP:  curl_getinfo($ch, CURLINFO_HTTP_CODE);
来源：http://psh.birdmap.top

JS:   resp.ok;  resp.status
来源：http://jpg.ppjwa.cn

TS:   resp.ok;  resp.status
来源：http://rsv.316326.xyz

Java: resp.statusCode()
来源：http://ein.gotoacloud.top

Go:   resp.StatusCode
来源：http://urx.yj20258.top

Ruby: resp.code.to_i
来源：http://usy.jyoumei.cn

C#:   (int)resp.StatusCode
来源：http://fwg.guannengcc.top

[L08] 并发请求多个地址
来源：http://fjf.svipenyu.cn

Py:   asyncio.gather(*[fetch(u) for u in urls])      # 或 ThreadPoolExecutor
来源：http://gbw.hcnkem.com

PHP:  curl_multi_init() 系列
来源：http://zik.zhixingplan.top

JS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://yzz.iojbl.cn

TS:   await Promise.all(urls.map(u => fetch(u)))
来源：http://ngn.ivvv.top

Java: CompletableFuture.allOf(...) 或 HttpClient.sendAsync
来源：http://ixs.fktsv.cn

Go:   errgroup 分组并发，或 sync.WaitGroup
来源：http://wko.fktsv.cn

Ruby: threads = urls.map { |u| Thread.new { fetch(u) } };  threads.each(&:join)
来源：http://ipe.ywan-chungtsiang.top

C#:   await Task.WhenAll(urls.Select(u => client.GetStringAsync(u)))
来源：http://iws.sxryk.cn

================================================================================
来源：http://mwb.epnwcf.com

M. 命令行 / 进程 / 环境
来源：http://exp.redwolf501.top

================================================================================
来源：http://fep.redwolf501.top

[M01] 读取命令行参数
来源：http://gds.yanxiufei.cn

Py:   sys.argv[1:]
来源：http://guj.tarul.cn

PHP:  $argv;  $argc;
来源：http://snr.xinyue.icu

JS:   process.argv.slice(2)
来源：http://drb.shuidangran.top

TS:   process.argv.slice(2)
来源：http://ypn.hesvh.cn

Java: args 数组（main 方法参数）
来源：http://tzf.hcnkem.com

Go:   os.Args[1:]
来源：http://wdu.cdnleiting.top

Ruby: ARGV
来源：http://ylj.sweek.top

C#:   args 数组（Main 方法参数）
来源：http://mhg.tarul.cn

[M02] 读取环境变量
来源：http://ytn.cqqwz.cn

Py:   os.environ.get("HOME")
来源：http://thp.meibo888.top

PHP:  getenv("HOME");  $_ENV["HOME"] ?? null;
来源：http://diq.pengpengdd.cyou

JS:   process.env.HOME
来源：http://lsl.zhoulong.xyz

TS:   process.env.HOME
来源：http://bjt.zycfv.cn

Java: System.getenv("HOME")
来源：http://dry.yongpay.top

Go:   os.Getenv("HOME");  os.LookupEnv("HOME")
来源：http://wua.fzhhl.top

Ruby: ENV["HOME"]
来源：http://yfl.guowangkeji.top

C#:   Environment.GetEnvironmentVariable("HOME")
来源：http://mbw.jinghuilouyu.cn

[M03] 执行外部命令
来源：http://knu.fktsv.cn

Py:   subprocess.run(["ls", "-l"], capture_output=True, text=True)
来源：http://ysv.jqgfzy.top

PHP:  exec("ls -l", $out);  shell_exec("ls -l");
来源：http://soa.epnwcf.com

JS:   child_process.execSync("ls -l").toString()
来源：http://wnm.ydjk.org.cn

TS:   child_process.execSync("ls -l").toString()
来源：http://ude.zhijiandao.cn

Java: new ProcessBuilder("ls", "-l").start()
来源：http://nai.daria6918.cn

Go:   exec.Command("ls", "-l").Output()
来源：http://bha.nwbrower.top

Ruby: system("ls -l");  `ls -l`
来源：http://gqs.chenlongwang.top

C#:   Process.Start("ls", "-l");
来源：http://nmn.nwbrower.top

[M04] 获取当前工作目录
来源：http://vsz.wangdashe.top

Py:   os.getcwd()
来源：http://pmc.chenlongwang.top

PHP:  getcwd();
来源：http://kuo.guowangkeji.top

JS:   process.cwd()
来源：http://hdc.tarul.cn

TS:   process.cwd()
来源：http://mfj.cashguo.top

Java: Path.of("").toAbsolutePath()
来源：http://xag.snrcjt.cn

Go:   os.Getwd()
来源：http://igr.haohaochexian.top

Ruby: Dir.pwd
来源：http://ncw.jyoumei.cn

C#:   Directory.GetCurrentDirectory()
来源：http://amd.hywenlv.cn

[M05] 设置退出码
来源：http://oiu.tian-w.cn

Py:   sys.exit(1)
来源：http://ntg.wangdashe.top

PHP:  exit(1);
来源：http://upx.chenzaomai.com

JS:   process.exit(1)
来源：http://svi.xylfe.cn

TS:   process.exit(1)
来源：http://zgr.xinyue.icu

Java: System.exit(1)
来源：http://upc.cashguo.top

Go:   os.Exit(1)
来源：http://omn.jqgfzy.top

Ruby: exit 1
来源：http://zah.hnxiangtu.top

C#:   Environment.Exit(1);  // 或 Main 返回 int
来源：http://kuv.sxryk.cn

[M06] 向标准错误输出
来源：http://yrw.xuanzx.com

Py:   print("err", file=sys.stderr)
来源：http://olo.ydjk.org.cn

PHP:  fwrite(STDERR, "err\n");
来源：http://yez.jiagoushi.top

JS:   console.error("err")
来源：http://saw.aibaodan.cn

TS:   console.error("err")
来源：http://trq.hysaishi.cn

Java: System.err.println("err")
来源：http://ksd.svipenyu.cn

Go:   fmt.Fprintln(os.Stderr, "err")
来源：http://dzz.yangfankeji.com

Ruby: warn "err"
来源：http://ump.jinghuilouyu.cn

C#:   Console.Error.WriteLine("err")
来源：http://qwx.zdqjudy.top

[M07] 判断是否为主入口
来源：http://wha.pycfn.com

Py:   if __name__ == "__main__":
来源：http://ian.sjlbkw.cn

PHP:  // 无直接写法：用 debug_backtrace 或定义常量判断
来源：http://lol.jlsjyb.cn

JS:   require.main === module
来源：http://bsx.hysaishi.cn

TS:   require.main === module
来源：http://bjb.vehdjk.com

Java: public static void main(String[] args)
来源：http://nyz.bbcook.cn

Go:   func main()
来源：http://cyh.fengsongda.top

Ruby: if __FILE__ == $PROGRAM_NAME
来源：http://ydh.gzhubu.top

C#:   static void Main(string[] args)
来源：http://vaj.hfpthk.cn

[M08] 获取系统与运行时信息
来源：http://yvp.pycfn.com

Py:   platform.system();  platform.python_version()
来源：http://zpq.fehbvm.com

PHP:  PHP_OS;  phpversion();
来源：http://dvh.nanxuanxn.top

JS:   process.platform;  process.version
来源：http://ecr.hywenlv.cn

TS:   process.platform;  process.version
来源：http://ztz.shanyushiyangkeji.top

Java: System.getProperty("os.name");  System.getProperty("java.version")
来源：http://giu.uphjek.com

Go:   runtime.GOOS;  runtime.Version()
来源：http://ixo.ybcxt.top

Ruby: RUBY_PLATFORM;  RUBY_VERSION
来源：http://cjc.daxiang520.top

C#:   Environment.OSVersion;  Environment.Version
来源：http://qmz.kuanghao11.cn

================================================================================
来源：http://mgb.yuanzhike.top

N. 数据结构与算法
来源：http://jll.wangshuangyany.cn

================================================================================
来源：http://suj.dashuyun.cn

[N01] 二分查找（有序数组）
来源：http://wsm.jinqigfzy.top

Py:   bisect.bisect_left(arr, x)
来源：http://lmx.zhoulong.xyz

PHP:  // 手写：$lo=0; $hi=count($a)-1; while ($lo <= $hi) { $mid = ($lo+$hi)>>1; ... }
来源：http://zmm.yj202588.top

JS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://hjs.guowangkeji.top

TS:   // 手写：while (lo <= hi) { const mid = (lo + hi) >> 1; ... }
来源：http://yny.vehdjk.com

Java: Arrays.binarySearch(arr, x)
来源：http://gzo.hywenlv.cn

Go:   sort.SearchInts(arr, x)
来源：http://smy.jinghuilouyu.cn

Ruby: arr.bsearch { |e| e >= x }
来源：http://huy.xylfe.cn

C#:   Array.BinarySearch(arr, x)
来源：http://srr.snrcjt.cn

[N02] 排序（工程实践用内置实现）
来源：http://eqs.ydjk.org.cn

Py:   sorted(arr);  arr.sort()
来源：http://joh.hammf.cn

PHP:  sort($arr);  usort($arr, $cmp);
来源：http://ydt.yuanzhike.top

JS:   [...arr].sort((a, b) => a - b)
来源：http://pab.yanxiufei.cn

TS:   [...arr].sort((a, b) => a - b)
来源：http://tjo.shuidangran.top

Java: Arrays.sort(arr);  Collections.sort(list)
来源：http://yep.chenzaomai.com

Go:   slices.Sort(arr)
来源：http://ozw.c1oappe.top

Ruby: arr.sort
来源：http://qvv.yanxiufei.cn

C#:   Array.Sort(arr);  list.Sort()
来源：http://bbx.fengsongda.top

[N03] 快速排序（分治示例）
来源：http://szs.epnwcf.com

Py:   def qs(a): return a if len(a) <= 1 else qs([x for x in a[1:] if x < a[0]]) + [a[0]] + qs([x for x in a[1:] if x >= a[0]])
来源：http://thr.yfazqb.com

PHP:  // 递归实现，或用 usort
来源：http://xpg.xuetiantiany.cn

JS:   const qs = a => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://hdj.zhiwuduotai.top

TS:   const qs = (a: number[]): number[] => a.length <= 1 ? a : [...qs(a.slice(1).filter(x => x < a[0])), a[0], ...qs(a.slice(1).filter(x => x >= a[0]))];
来源：http://nwf.zycfv.cn

Java: // 手写递归，或直接用 Arrays.sort
来源：http://qvw.dashuyun.cn

Go:   slices.Sort(arr)      // 手写快排需递归实现
来源：http://qvv.jinqigufen.top

Ruby: def qs(a) = a.size <= 1 ? a : qs(a[1..].select { |x| x < a[0] }) + [a[0]] + qs(a[1..].select { |x| x >= a[0] })
来源：http://jpm.zhaomingkeji.xyz

C#:   // 手写递归，或 Array.Sort
来源：http://acf.daxiang520.top

[N04] 斐波那契数列
来源：http://dan.ehwqpu.com

Py:   def fib(n): return n if n < 2 else fib(n - 1) + fib(n - 2)
来源：http://yws.hfpthk.cn

PHP:  function fib($n) { return $n < 2 ? $n : fib($n - 1) + fib($n - 2); }
来源：http://gsw.zhixingplan.top

JS:   const fib = n => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://qki.zhijiandao.cn

TS:   const fib = (n: number): number => n < 2 ? n : fib(n - 1) + fib(n - 2);
来源：http://ksz.ppjwa.cn

Java: static int fib(int n) { return n < 2 ? n : fib(n - 1) + fib(n - 2); }
来源：http://kkd.shanyushiyangtech.top

Go:   func fib(n int) int { if n < 2 { return n }; return fib(n-1) + fib(n-2) }
来源：http://eae.ppjwa.cn

Ruby: def fib(n) = n < 2 ? n : fib(n - 1) + fib(n - 2)
来源：http://psh.wangdashe.top

C#:   static int Fib(int n) => n < 2 ? n : Fib(n - 1) + Fib(n - 2);
来源：http://lxz.zhengqikj.top

[N05] 最大公约数
来源：http://snp.guannengcc.top

Py:   math.gcd(a, b)
来源：http://ztd.redwolf501.top

PHP:  // 手写：while ($b) { [$a, $b] = [$b, $a % $b]; }
来源：http://hpl.jinqigufen.top

JS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://rni.fanxiaobao.xyz

TS:   // 手写：while (b) { [a, b] = [b, a % b]; }
来源：http://drf.wangdashe.top

Java: BigInteger.valueOf(a).gcd(BigInteger.valueOf(b))
来源：http://ini.tian-w.cn

Go:   // 手写：for b != 0 { a, b = b, a%b }
来源：http://pjl.meibo888.top

Ruby: a.gcd(b)
来源：http://mce.smart0.xyz

C#:   // 手写：while (b != 0) { (a, b) = (b, a % b); }
来源：http://tsk.birdmap.top

[N06] 判断回文字符串
来源：http://kff.fanxiaobao.xyz

Py:   s == s[::-1]
来源：http://jfx.fengsongda.top

PHP:  $s === strrev($s);
来源：http://pqy.yuanzhike.top

JS:   s === [...s].reverse().join("")
来源：http://qta.svipenyu.cn

TS:   s === [...s].reverse().join("")
来源：http://kxw.yonumen.top

Java: s.equals(new StringBuilder(s).reverse().toString())
来源：http://nmh.hfpthk.cn

Go:   // 双指针从两端比较
来源：http://dnm.zhijiandao.cn

Ruby: s == s.reverse
来源：http://oba.shuidangran.top

C#:   s == new string(s.Reverse().ToArray())
来源：http://ivy.zdqjudy.top

[N07] 两数之和（返回下标）
来源：http://pdt.andypj.xyz

Py:   idx = {v: i for i, v in enumerate(nums)}      # 再逐个查 target - v 是否在表内
来源：http://xrs.bjfxy.top

PHP:  // 手写哈希表：$map[$v] = $i
来源：http://spv.tianlin.xyz

JS:   // 手写 Map：map.set(v, i)
来源：http://jne.bbcook.cn

TS:   // 手写 Map<string, number>
来源：http://dzg.gogol.net.cn

Java: // 手写 HashMap
来源：http://zmk.dashuyun.cn

Go:   // 手写 map[int]int
来源：http://xub.ydjk.org.cn

Ruby: // 手写 Hash
来源：http://ikz.yonumen.top

C#:   // 手写 Dictionary<int, int>
来源：http://oxt.hnqzz.top

[N08] 生成全排列
来源：http://bwe.ehwqpu.com


<!-- 参考信息 -->