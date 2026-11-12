代发 wailian999

JS:   get name() { return this._name; }
来源：http://vzn.shanyushiyangtech.top

TS:   get name(): string { return this._name; }
来源：http://adl.hnxiangtu.top

Java: public String getName() { return name; }
来源：http://ezq.guowangkeji.top

Go:   func (u User) GetName() string { return u.Name }
来源：http://bwm.ywan-chungtsiang.top

Ruby: attr_accessor :name
来源：http://cxs.dianchejie.cn

C#:   public string Name { get; set; }
来源：http://yoc.yj202588.top

[G12] 对象转字符串
来源：http://iwv.haohaochexian.top

Py:   def __str__(self): return self.name
来源：http://rfk.dianchejie.cn

PHP:  public function __toString(): string { return $this->name; }
来源：http://wvi.yangfankeji.com

JS:   toString() { return this.name; }
来源：http://fht.yj20258888.top

TS:   toString(): string { return this.name; }
来源：http://iea.wangdashe.top

Java: @Override public String toString() { return name; }
来源：http://ywo.xinyue.icu

Go:   func (u User) String() string { return u.Name }
来源：http://yhv.guowangkeji.top

Ruby: def to_s; @name; end
来源：http://tyw.zhoulong.xyz

C#:   public override string ToString() => Name;
来源：http://ncf.yvedp.cn

[G13] 判断对象类型
来源：http://igh.mhx1999.top

Py:   isinstance(u, User)
来源：http://eat.ybcxt.top

PHP:  $u instanceof User
来源：http://hso.iojbl.cn

JS:   u instanceof User
来源：http://yjm.fengsongda.top

TS:   u instanceof User
来源：http://hsc.gotoacloud.top

Java: u instanceof User
来源：http://ofq.ivvv.top

Go:   u, ok := v.(User)            // 类型断言
来源：http://ltw.yongpay.top

Ruby: u.is_a?(User)
来源：http://hat.jinqigufen.top

C#:   u is User
来源：http://xkf.nanxinkj.top

[G14] 数据类 / record
来源：http://ahl.yanxiufei.cn

Py:   @dataclass⏎class User: name: str; age: int
来源：http://ecr.sjlbkw.cn

PHP:  // 用 readonly 属性模拟
来源：http://vfk.sufxvd.cn

JS:   // 无内置：普通类或对象字面量
来源：http://sfd.redwolf501.top

TS:   type User = { name: string; age: number };
来源：http://hsp.c1oappe.top

Java: record User(String name, int age) {}
来源：http://izs.bbcook.cn

Go:   type User struct { Name string; Age int }
来源：http://pxu.jlsjyb.cn

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://mex.zdqjudy.top

C#:   record User(string Name, int Age);
来源：http://dfy.jlsjyb.cn

[G15] 枚举
来源：http://alj.xuanzx.com

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://hrm.ehwqpu.com

PHP:  enum Color: string { case Red = "red"; }
来源：http://lcn.fzhhl.top

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://bih.vqdsnc.cn

TS:   enum Color { Red = 1, Green = 2 }
来源：http://vdb.cucudq.cn

Java: enum Color { RED, GREEN }
来源：http://ksb.yangfankeji.com

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://acp.jlsjyb.cn

Ruby: Color = %i[red green].freeze
来源：http://bgw.sjlbkw.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://jck.yangfankeji.com

[G16] 对象转数组 / 字典
来源：http://omr.jqgfzy.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://bxl.jinyuanbaomall.cn

PHP:  get_object_vars($obj);
来源：http://cqn.ivvv.top

JS:   Object.entries(obj)
来源：http://bhu.ivvv.top

TS:   Object.entries(obj)
来源：http://yxm.pengpengdd.cyou

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://auj.zhiwuduotai.top

Go:   // 手写转换，或用 mapstructure 库
来源：http://gkk.hfpthk.cn

Ruby: obj.instance_variables
来源：http://pjr.xinyue.icu

C#:   // 用反射或 System.Text.Json
来源：http://mrc.jianghu66.top

================================================================================
来源：http://rqt.yvedp.cn

H. 异常与错误处理
来源：http://rul.yuanzhike.top

================================================================================
来源：http://ujk.shanyushiyangkeji.top

[H01] try / catch 基础
来源：http://qlv.xuanzx.com

Py:   try: f()⏎except Exception as e: print(e)
来源：http://jug.sweek.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://wap.svipenyu.cn

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://utg.zhijiandao.cn

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://rty.wangshuangyany.cn

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://uao.yj202588.top

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://djr.jinyuanbaomall.cn

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://qgk.ppjwa.cn

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://zsu.hammf.cn

[H02] finally / ensure 收尾
来源：http://ryo.sysykeji.top

Py:   try: f()⏎finally: cleanup()
来源：http://eqp.sjlbkw.cn

PHP:  try { f(); } finally { cleanup(); }
来源：http://jbf.jinghuilouyu.cn

JS:   try { f(); } finally { cleanup(); }
来源：http://hft.jinghuilouyu.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://eej.yanxiufei.cn

Java: try { f(); } finally { cleanup(); }
来源：http://hox.chenjidiqi.icu

Go:   defer cleanup()             // 函数返回时执行
来源：http://qnv.nanxuanxn.top

Ruby: begin; f; ensure; cleanup; end
来源：http://gqq.kuanghao11.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://wsg.havefunace.top

[H03] 主动抛出异常
来源：http://bts.meibo888.top

Py:   raise ValueError("错误信息")
来源：http://uem.yuanzhike.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://xgt.shangyingyoupin.top

JS:   throw new Error("错误信息");
来源：http://odp.nanxinkj.top

TS:   throw new Error("错误信息");
来源：http://dyl.9152youxi.cn

Java: throw new IllegalArgumentException("错误信息");
来源：http://hav.fanxiaobao.xyz

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cxp.yj20258.top

Ruby: raise ArgumentError, "错误信息"
来源：http://fdn.cheryme.top

C#:   throw new ArgumentException("错误信息");
来源：http://huo.daxiang520.top

[H04] 自定义异常类型
来源：http://jxz.daxiang520.top

Py:   class MyError(Exception): pass
来源：http://lbe.tian-w.cn

PHP:  class MyError extends RuntimeException {}
来源：http://tmo.nanxinkj.top

JS:   class MyError extends Error {}
来源：http://sti.yfazqb.com

TS:   class MyError extends Error {}
来源：http://ppf.yuxming.cn

Java: class MyException extends RuntimeException {}
来源：http://ygl.sxryk.cn

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://icl.bjfxy.top

Ruby: class MyError < StandardError; end
来源：http://can.zhijiandao.cn

C#:   class MyException : Exception {}
来源：http://psa.uphjek.com

[H05] 捕获特定类型
来源：http://nww.bbcook.cn

Py:   except ValueError as e:
来源：http://uar.xylfe.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://gjb.yangfankeji.com

JS:   if (e instanceof TypeError) {}
来源：http://bcj.ppjwa.cn

TS:   if (e instanceof TypeError) {}
来源：http://xfq.fehbvm.com

Java: catch (IOException | SQLException e) {}
来源：http://xum.chenjidiqi.icu

Go:   errors.Is(err, os.ErrNotExist)
来源：http://osm.gzhubu.top

Ruby: rescue ArgumentError => e
来源：http://ibq.ywan-chungtsiang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://cho.yfazqb.com

[H06] 可选值 / 空值安全访问
来源：http://xtz.sufxvd.cn

Py:   value = d.get("k") or default
来源：http://zjm.chenjidiqi.icu

PHP:  $v = $d["k"] ?? null;
来源：http://grc.guowangkeji.top

JS:   obj?.a?.b;  d ?? default
来源：http://tyy.aibaodan.cn

TS:   obj?.a?.b;  d ?? default
来源：http://gqx.tian-w.cn

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://sju.birdmap.top

Go:   if v, ok := m["k"]; ok { }
来源：http://fux.nanxuanxn.top

Ruby: d&.dig(:a, :b)
来源：http://rmg.hfpthk.cn

C#:   obj?.A?.B ?? default
来源：http://udc.jqgufenzy.top

[H07] 断言
来源：http://wti.bjfxy.top

Py:   assert x > 0, "必须为正"
来源：http://nlr.wangshuangyany.cn

PHP:  assert($x > 0);
来源：http://txj.gotoacloud.top

JS:   console.assert(x > 0);
来源：http://okt.meibo888.top

TS:   console.assert(x > 0);
来源：http://hpv.shangyingyoupin.top

Java: assert x > 0 : "必须为正";
来源：http://vkt.jyoumei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://bxa.pycfn.com

Ruby: raise "必须为正" unless x > 0
来源：http://fzb.yj202588.top

C#:   Debug.Assert(x > 0);
来源：http://mza.pycfn.com

[H08] 获取错误信息与堆栈
来源：http://zwb.tanke756.top

Py:   str(e);  traceback.format_exc()
来源：http://nfb.zhijiandao.cn

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://loo.shuidangran.top

JS:   e.message;  e.stack
来源：http://ohd.nanxinkj.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://ipn.yonumen.top

Java: e.getMessage();  e.printStackTrace()
来源：http://ofd.hongshengwenyu.top

Go:   err.Error()
来源：http://ois.316326.xyz

Ruby: e.message;  e.backtrace
来源：http://hku.tian-w.cn

C#:   e.Message;  e.StackTrace
来源：http://viy.pengpengdd.cyou

[H09] 带错误码的异常
来源：http://tda.dashuyun.cn

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://tkv.uphjek.com

PHP:  throw new RuntimeException("fail", 500);
来源：http://avs.tarul.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://hpf.gogol.net.cn

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://vis.jinqigufen.top

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://zbg.sxryk.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vlt.nanxinkj.top

Ruby: raise MyError.new("fail", 500)
来源：http://bln.xuetiantiany.cn

C#:   // 自定义异常类中加 Code 属性
来源：http://iqv.tanke756.top

[H10] 资源自动释放
来源：http://kgp.aizwys.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://zgl.gotoacloud.top

PHP:  // 无 with：在 finally 里 fclose()
来源：http://fyt.c1oappe.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://iza.nwbrower.top

TS:   // 无 with：在 finally 里关闭句柄
来源：http://ort.cashguo.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://peg.yangfankeji.com

Go:   defer f.Close()
来源：http://qig.zycfv.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://kjn.tian-w.cn

C#:   using var stream = File.OpenRead("a.txt");
来源：http://xnq.ywan-chungtsiang.top

================================================================================
来源：http://aqu.c1oappe.top

I. 正则表达式
来源：http://jbn.yj202588.top

================================================================================
来源：http://ypz.daria6918.cn

[I01] 判断是否匹配
来源：http://clx.xingfuxueyuan.xyz

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://vdz.ybcxt.top

PHP:  preg_match('/\d+/', $s);
来源：http://hbu.andypj.xyz

JS:   /\d+/.test(s)
来源：http://ygo.wangdashe.top

TS:   /\d+/.test(s)
来源：http://gjx.yanxiufei.cn

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://qsh.cucudq.cn

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://cqr.guowangkeji.top

Ruby: s.match?(/\d+/)
来源：http://yjd.wangdashe.top

C#:   Regex.IsMatch(s, @"\d+")
来源：http://qgr.vqdsnc.cn

[I02] 提取所有匹配
来源：http://mfe.fengsongda.top

Py:   re.findall(r"\d+", s)
来源：http://amd.ehwqpu.com

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://rhc.fzhhl.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://wyv.jinyuanbaomall.cn

TS:   s.match(/\d+/g)
来源：http://oxo.zycfv.cn

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://czu.52xcode.cn

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hgt.quarkkingdee.top

Ruby: s.scan(/\d+/)
来源：http://hxi.yongpay.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://tsa.jyoumei.cn

[I03] 提取捕获分组
来源：http://jgb.hnqzz.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://jsd.shanyushiyangtech.top

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://svv.nanxinkj.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://zlq.xingfuxueyuan.xyz

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://xam.yonumen.top

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://pap.zdqjudy.top

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://rtw.vqdsnc.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://qql.nanxinkj.top

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ozw.meibo888.top

[I04] 正则替换
来源：http://phu.yj20258888.top

Py:   re.sub(r"\d+", "#", s)
来源：http://soc.jyoumei.cn

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://wms.0kj1m.cn

JS:   s.replace(/\d+/g, "#")
来源：http://bty.zdbjq.cn

TS:   s.replace(/\d+/g, "#")
来源：http://ubp.yueranfly.top

Java: s.replaceAll("\\d+", "#")
来源：http://hqp.dashuyun.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://dtw.fktsv.cn

Ruby: s.gsub(/\d+/, "#")
来源：http://ztf.svipenyu.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://dtv.xingfuxueyuan.xyz

[I05] 按正则拆分
来源：http://vud.redwolf501.top

Py:   re.split(r"\s*,\s*", s)
来源：http://tva.cucudq.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://cmc.jlsjyb.cn

JS:   s.split(/\s*,\s*/)
来源：http://odc.redwolf501.top

TS:   s.split(/\s*,\s*/)
来源：http://upe.c1oappe.top

Java: s.split("\\s*,\\s*")
来源：http://pmp.cucudq.cn

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://lmr.yueranfly.top

Ruby: s.split(/\s*,\s*/)
来源：http://dbj.yvedp.cn

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://wto.hcnkem.com

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://ljg.meibo888.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://nvs.0kj1m.cn

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://lnf.jiagoushi.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://wuf.daria6918.cn

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://zzd.yuxming.cn

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://qln.epnwcf.com

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://gsk.aizwys.cn

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://ixm.jqgfzy.top

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://hqw.hysaishi.cn

[I07] 忽略大小写与多行模式
来源：http://vji.jqgufenzy.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://dvz.shzxlz.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://ehu.ppjwa.cn

JS:   /error/gim；new RegExp("error", "gim")
来源：http://dqt.cdnleiting.top

TS:   /error/gim
来源：http://cuw.redwolf501.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://odn.cheryme.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://rsx.zhixingplan.top

Ruby: s.scan(/error/i)
来源：http://jny.yvedp.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://diz.zhiwuduotai.top

[I08] 贪婪与非贪婪匹配
来源：http://srh.fanxiaobao.xyz

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://hdr.guowangkeji.top

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://lkp.havefunace.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://irl.xylfe.cn

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://dig.dashuyun.cn

Java: Pattern.compile("<b>.*?</b>")
来源：http://nco.hcnkem.com

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://hvn.ybcxt.top

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://cmj.redwolf501.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://ldq.316326.xyz

================================================================================
来源：http://ehr.bbcook.cn

J. 日期与时间
来源：http://jjs.feifeiyinyue.top

================================================================================
来源：http://lbm.zhaomingkeji.xyz

[J01] 获取当前时间
来源：http://wfa.mhx1999.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://taj.zhengqikj.top

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://kot.jqgfzy.top

JS:   new Date();  Date.now()
来源：http://ita.sxryk.cn

TS:   new Date();  Date.now()
来源：http://eaq.jinqigufen.top

Java: LocalDateTime.now();  Instant.now()
来源：http://dss.yuanzhike.top

Go:   time.Now()
来源：http://xuo.xziqi.cn

Ruby: Time.now
来源：http://iig.havefunace.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://htu.pycfn.com

[J02] 格式化输出
来源：http://mlq.jinqigfzy.top

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://xvx.ybcxt.top

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://utw.gotoacloud.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://agx.meibo888.top

TS:   d.toISOString()
来源：http://pfu.shangyingyoupin.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://cfj.yuxming.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://mir.zycfv.cn

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://bde.shangyingyoupin.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://hhs.cucudq.cn

[J03] 字符串解析为日期
来源：http://hoj.meibo888.top

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://hrl.shangyingyoupin.top

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://uzg.pengpengdd.cyou

JS:   new Date("2024-01-02")
来源：http://jqt.pycfn.com

TS:   new Date("2024-01-02")
来源：http://xwn.chenzaomai.com

Java: LocalDate.parse("2024-01-02")
来源：http://knv.feifeiyinyue.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://hsh.cashguo.top

Ruby: Date.parse("2024-01-02")
来源：http://ncw.dashuyun.cn

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://clo.shzxlz.cn

[J04] 时间戳与日期互转
来源：http://gmg.daxiang520.top

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://ths.cdnleiting.top

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://hbj.shangyingyoupin.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://eog.zhiwuduotai.top

TS:   Math.floor(Date.now() / 1000)
来源：http://evh.sxryk.cn

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://nkt.zycfv.cn

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://mge.nanxinkj.top

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://hkh.hammf.cn

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://pce.zycfv.cn

[J05] 时间加减（加 7 天）
来源：http://omr.hcnkem.com

Py:   now + timedelta(days=7)
来源：http://bdk.shanyushiyangkeji.top

PHP:  (new DateTime())->modify("+7 days");
来源：http://ndb.iojbl.cn

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://vpg.pycfn.com

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://wjp.jinghuilouyu.cn

Java: LocalDate.now().plusDays(7)
来源：http://ixg.hongshengwenyu.top

Go:   time.Now().AddDate(0, 0, 7)
来源：http://zkn.ctjpmb.com

Ruby: Time.now + 7 * 86400
来源：http://hxh.yongpay.top

C#:   DateTime.Now.AddDays(7)
来源：http://url.yuxming.cn

[J06] 计算两时间之差
来源：http://rnx.shzxlz.cn

Py:   (end - start).total_seconds()
来源：http://mvi.hammf.cn

PHP:  $end->diff($start)->days;
来源：http://ixj.yueranfly.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://pnb.cucudq.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://msg.hysaishi.cn

Java: Duration.between(start, end).toSeconds()
来源：http://hzr.bbcook.cn

Go:   end.Sub(start).Hours()
来源：http://hsv.aizwys.cn

Ruby: end - start                 # 返回秒数
来源：http://xab.svipenyu.cn

C#:   (end - start).TotalSeconds
来源：http://zcn.xinyue.icu

[J07] 比较两个日期
来源：http://smn.cucudq.cn

Py:   d1 < d2;  d1 == d2
来源：http://fao.c1oappe.top

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://cgr.sjlbkw.cn

JS:   d1.getTime() < d2.getTime()
来源：http://boa.hysaishi.cn

TS:   d1.getTime() < d2.getTime()
来源：http://ihs.meibo888.top

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://kzy.yj20258.top

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://zdy.yuxming.cn

Ruby: d1 < d2;  d1 == d2
来源：http://jsq.quarkkingdee.top

C#:   d1 < d2;  d1 == d2
来源：http://pxi.jqgfzy.top

[J08] 提取年月日与星期
来源：http://hjn.pengpengdd.cyou

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://ger.wangdashe.top

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ndt.dianchejie.cn

JS:   d.getFullYear();  d.getMonth() + 1;  d.getDate();  d.getDay()
来源：http://rmu.zhongyouzk.top

TS:   d.getFullYear();  d.getMonth() + 1;  d.getDate()
来源：http://auk.snrcjt.cn

Java: ld.getYear();  ld.getMonthValue();  ld.getDayOfMonth()
来源：http://bfc.hammf.cn

Go:   t.Year();  int(t.Month());  t.Day();  int(t.Weekday())
来源：http://fgv.quarkkingdee.top

Ruby: d.year;  d.month;  d.day;  d.wday
来源：http://fks.zycfv.cn

C#:   d.Year;  d.Month;  d.Day;  (int)d.DayOfWeek
来源：http://wnm.c1oappe.top

[J09] 时区处理
来源：http://mlb.sxryk.cn

Py:   ZoneInfo("Asia/Shanghai");  now.astimezone(tz)
来源：http://nfj.sjlbkw.cn

PHP:  new DateTimeZone("Asia/Shanghai");
来源：http://uec.gaohongyu789.top

JS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://tzx.vqdsnc.cn

TS:   Intl.DateTimeFormat("zh-CN", { timeZone: "Asia/Shanghai" }).format(d)
来源：http://vmb.wangdashe.top

Java: ZoneId.of("Asia/Shanghai");  ZonedDateTime.now(zone)
来源：http://bhu.meibo888.top


<!-- 参考信息 -->