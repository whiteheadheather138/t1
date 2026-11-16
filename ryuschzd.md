代发 wailian999

[G10] 访问控制
来源：http://apu.yvedp.cn

Py:   约定 _protected / __private（不强制）
来源：http://phq.52xcode.cn

PHP:  public / protected / private
来源：http://xap.xuanzx.com

JS:   #private 字段；其余公开
来源：http://cou.birdmap.top

TS:   public / protected / private
来源：http://gsr.redwolf501.top

Java: public / protected / private / 默认包级
来源：http://yew.gotoacloud.top

Go:   首字母大写可导出，小写仅包内可见
来源：http://dqi.kuanghao11.cn

Ruby: public / protected / private
来源：http://jud.jinghuilouyu.cn

C#:   public / protected / private / internal
来源：http://kpu.epnwcf.com

[G11] getter / setter
来源：http://vfa.hongshengwenyu.top

Py:   @property 与 @x.setter
来源：http://tgm.mhx1999.top

PHP:  public function getName(): string { return $this->name; }
来源：http://ysd.zdqjudy.top

JS:   get name() { return this._name; }
来源：http://iqj.guowangkeji.top

TS:   get name(): string { return this._name; }
来源：http://miq.iojbl.cn

Java: public String getName() { return name; }
来源：http://igp.sjlbkw.cn

Go:   func (u User) GetName() string { return u.Name }
来源：http://mpl.hnqzz.top

Ruby: attr_accessor :name
来源：http://een.wangdashe.top

C#:   public string Name { get; set; }
来源：http://vjt.yangfankeji.com

[G12] 对象转字符串
来源：http://rte.xylfe.cn

Py:   def __str__(self): return self.name
来源：http://drw.zhaomingkeji.xyz

PHP:  public function __toString(): string { return $this->name; }
来源：http://cem.pengpengdd.cyou

JS:   toString() { return this.name; }
来源：http://zgw.shanyushiyangkeji.top

TS:   toString(): string { return this.name; }
来源：http://amc.chenzaomai.com

Java: @Override public String toString() { return name; }
来源：http://jgu.redwolf501.top

Go:   func (u User) String() string { return u.Name }
来源：http://lvx.0kj1m.cn

Ruby: def to_s; @name; end
来源：http://ror.xziqi.cn

C#:   public override string ToString() => Name;
来源：http://qud.shanyushiyangkeji.top

[G13] 判断对象类型
来源：http://ecn.daria6918.cn

Py:   isinstance(u, User)
来源：http://ywg.snrcjt.cn

PHP:  $u instanceof User
来源：http://xza.hesvh.cn

JS:   u instanceof User
来源：http://ijv.zhiwuduotai.top

TS:   u instanceof User
来源：http://adg.guowangkeji.top

Java: u instanceof User
来源：http://fkj.xylfe.cn

Go:   u, ok := v.(User)            // 类型断言
来源：http://ebe.shanyushiyangkeji.top

Ruby: u.is_a?(User)
来源：http://gle.xingfuxueyuan.xyz

C#:   u is User
来源：http://uak.nanxuanxn.top

[G14] 数据类 / record
来源：http://uqr.hnxiangtu.top

Py:   @dataclass⏎class User: name: str; age: int
来源：http://kcn.iojbl.cn

PHP:  // 用 readonly 属性模拟
来源：http://cxg.cqqwz.cn

JS:   // 无内置：普通类或对象字面量
来源：http://zeg.nanxuanxn.top

TS:   type User = { name: string; age: number };
来源：http://fzo.daxiang520.top

Java: record User(String name, int age) {}
来源：http://lem.tian-w.cn

Go:   type User struct { Name string; Age int }
来源：http://ted.yfazqb.com

Ruby: User = Struct.new(:name, :age)   # 或 Ruby 3.2+ 的 Data.define
来源：http://fxs.dashuyun.cn

C#:   record User(string Name, int Age);
来源：http://ehp.vqdsnc.cn

[G15] 枚举
来源：http://lsi.chenjidiqi.icu

Py:   from enum import Enum;  class Color(Enum): RED = 1
来源：http://cpm.jinqigufen.top

PHP:  enum Color: string { case Red = "red"; }
来源：http://qdq.zhijiandao.cn

JS:   const Color = Object.freeze({ RED: 1, GREEN: 2 });
来源：http://emb.bjfxy.top

TS:   enum Color { Red = 1, Green = 2 }
来源：http://iwu.gogol.net.cn

Java: enum Color { RED, GREEN }
来源：http://gge.jinyuanbaomall.cn

Go:   type Color int;  const (Red Color = iota; Green)
来源：http://bfm.xziqi.cn

Ruby: Color = %i[red green].freeze
来源：http://xbe.cqqwz.cn

C#:   enum Color { Red = 1, Green = 2 }
来源：http://ral.fengsongda.top

[G16] 对象转数组 / 字典
来源：http://bwy.fzhhl.top

Py:   dataclasses.asdict(obj);  obj.__dict__
来源：http://vxt.birdmap.top

PHP:  get_object_vars($obj);
来源：http://ahl.shangyingyoupin.top

JS:   Object.entries(obj)
来源：http://cgp.meibo888.top

TS:   Object.entries(obj)
来源：http://osz.zdbjq.cn

Java: // 用 Jackson 等序列化库，或手写 toMap()
来源：http://ocg.tarul.cn

Go:   // 手写转换，或用 mapstructure 库
来源：http://bej.shanyushiyangtech.top

Ruby: obj.instance_variables
来源：http://qte.tanke756.top

C#:   // 用反射或 System.Text.Json
来源：http://hvx.316326.xyz

================================================================================
来源：http://aoi.epnwcf.com

H. 异常与错误处理
来源：http://yie.gzhubu.top

================================================================================
来源：http://eti.nanxuanxn.top

[H01] try / catch 基础
来源：http://mbj.xziqi.cn

Py:   try: f()⏎except Exception as e: print(e)
来源：http://kjw.zdqjudy.top

PHP:  try { f(); } catch (Exception $e) { echo $e->getMessage(); }
来源：http://daj.mhx1999.top

JS:   try { f(); } catch (e) { console.error(e); }
来源：http://bwj.jinqigfzy.top

TS:   try { f(); } catch (e: unknown) { console.error(e); }
来源：http://puc.chenjidiqi.icu

Java: try { f(); } catch (Exception e) { System.out.println(e.getMessage()); }
来源：http://bvc.zhijiandao.cn

Go:   if err := f(); err != nil { log.Println(err) }   // Go 用返回值而非异常
来源：http://mry.zdqjudy.top

Ruby: begin; f; rescue => e; puts e.message; end
来源：http://ymv.hnxiangtu.top

C#:   try { F(); } catch (Exception e) { Console.WriteLine(e.Message); }
来源：http://ebx.jlsjyb.cn

[H02] finally / ensure 收尾
来源：http://cpj.ydjk.org.cn

Py:   try: f()⏎finally: cleanup()
来源：http://fzg.gzhubu.top

PHP:  try { f(); } finally { cleanup(); }
来源：http://wpa.yuanzhike.top

JS:   try { f(); } finally { cleanup(); }
来源：http://yqp.yvedp.cn

TS:   try { f(); } finally { cleanup(); }
来源：http://xwh.bjfxy.top

Java: try { f(); } finally { cleanup(); }
来源：http://qvj.jinghuilouyu.cn

Go:   defer cleanup()             // 函数返回时执行
来源：http://yxp.gzhubu.top

Ruby: begin; f; ensure; cleanup; end
来源：http://bwl.hysaishi.cn

C#:   try { F(); } finally { Cleanup(); }
来源：http://rwa.shanyushiyangtech.top

[H03] 主动抛出异常
来源：http://fta.epnwcf.com

Py:   raise ValueError("错误信息")
来源：http://uhs.yuanzhike.top

PHP:  throw new InvalidArgumentException("错误信息");
来源：http://uhi.tian-w.cn

JS:   throw new Error("错误信息");
来源：http://xyw.snrcjt.cn

TS:   throw new Error("错误信息");
来源：http://lab.hcnkem.com

Java: throw new IllegalArgumentException("错误信息");
来源：http://vso.yangfankeji.com

Go:   return fmt.Errorf("错误信息: %w", err)
来源：http://cig.jqgfzy.top

Ruby: raise ArgumentError, "错误信息"
来源：http://hcg.xziqi.cn

C#:   throw new ArgumentException("错误信息");
来源：http://eet.shangyingyoupin.top

[H04] 自定义异常类型
来源：http://ykg.aibaodan.cn

Py:   class MyError(Exception): pass
来源：http://epl.wangshuangyany.cn

PHP:  class MyError extends RuntimeException {}
来源：http://ocf.hywenlv.cn

JS:   class MyError extends Error {}
来源：http://wnj.wangdashe.top

TS:   class MyError extends Error {}
来源：http://srl.xinyue.icu

Java: class MyException extends RuntimeException {}
来源：http://jpc.nanxinkj.top

Go:   type MyError struct{ Msg string };  func (e MyError) Error() string { return e.Msg }
来源：http://iaj.ydzc1.top

Ruby: class MyError < StandardError; end
来源：http://awl.jianghu66.top

C#:   class MyException : Exception {}
来源：http://pat.ydzc1.top

[H05] 捕获特定类型
来源：http://gob.dianchejie.cn

Py:   except ValueError as e:
来源：http://xnq.0kj1m.cn

PHP:  catch (InvalidArgumentException | RuntimeException $e) {}   // 支持多类型
来源：http://ewu.haohaochexian.top

JS:   if (e instanceof TypeError) {}
来源：http://ajz.bbcook.cn

TS:   if (e instanceof TypeError) {}
来源：http://lcx.vqdsnc.cn

Java: catch (IOException | SQLException e) {}
来源：http://yht.fanxiaobao.xyz

Go:   errors.Is(err, os.ErrNotExist)
来源：http://prl.smart0.xyz

Ruby: rescue ArgumentError => e
来源：http://aol.chenlongwang.top

C#:   catch (IOException e) when (e.HResult == -1) {}
来源：http://ilc.fehbvm.com

[H06] 可选值 / 空值安全访问
来源：http://rct.jqgufenzy.top

Py:   value = d.get("k") or default
来源：http://qcc.zhengqikj.top

PHP:  $v = $d["k"] ?? null;
来源：http://swv.yanxiufei.cn

JS:   obj?.a?.b;  d ?? default
来源：http://wew.wangshuangyany.cn

TS:   obj?.a?.b;  d ?? default
来源：http://zwr.redwolf501.top

Java: Optional.ofNullable(x).map(...).orElse(default)
来源：http://umf.sweek.top

Go:   if v, ok := m["k"]; ok { }
来源：http://lzs.pengpengdd.cyou

Ruby: d&.dig(:a, :b)
来源：http://yqq.yuxming.cn

C#:   obj?.A?.B ?? default
来源：http://atd.gaohongyu789.top

[H07] 断言
来源：http://fmb.xuetiantiany.cn

Py:   assert x > 0, "必须为正"
来源：http://ysk.hongshengwenyu.top

PHP:  assert($x > 0);
来源：http://ily.ivvv.top

JS:   console.assert(x > 0);
来源：http://len.jyoumei.cn

TS:   console.assert(x > 0);
来源：http://wzq.dashuyun.cn

Java: assert x > 0 : "必须为正";
来源：http://yau.yanxiufei.cn

Go:   // 无 assert：手写 if 后 panic 或返回错误
来源：http://zjn.9152youxi.cn

Ruby: raise "必须为正" unless x > 0
来源：http://cis.kuanghao11.cn

C#:   Debug.Assert(x > 0);
来源：http://xrd.redwolf501.top

[H08] 获取错误信息与堆栈
来源：http://bth.pengpengdd.cyou

Py:   str(e);  traceback.format_exc()
来源：http://erf.ywan-chungtsiang.top

PHP:  $e->getMessage();  $e->getTraceAsString();
来源：http://foz.zycfv.cn

JS:   e.message;  e.stack
来源：http://vte.jqgfzy.top

TS:   e instanceof Error ? e.message : String(e)
来源：http://las.pengpengdd.cyou

Java: e.getMessage();  e.printStackTrace()
来源：http://ivg.vehdjk.com

Go:   err.Error()
来源：http://iku.yuanzhike.top

Ruby: e.message;  e.backtrace
来源：http://jrh.yanxiufei.cn

C#:   e.Message;  e.StackTrace
来源：http://qgt.gogol.net.cn

[H09] 带错误码的异常
来源：http://nwz.gaohongyu789.top

Py:   class HttpError(Exception):⏎    def __init__(self, msg, code): self.code = code
来源：http://nzm.shanyushiyangkeji.top

PHP:  throw new RuntimeException("fail", 500);
来源：http://iny.kuanghao11.cn

JS:   const err = new Error("fail");  err.code = 500;
来源：http://bgr.chenjidiqi.icu

TS:   class HttpError extends Error { constructor(public status: number) { super("fail"); } }
来源：http://jnx.xziqi.cn

Java: class HttpException extends RuntimeException { private final int code; }
来源：http://aaa.sjlbkw.cn

Go:   return fmt.Errorf("%w", ErrNotFound)     // 用 sentinel error 判断
来源：http://vlb.fengsongda.top

Ruby: raise MyError.new("fail", 500)
来源：http://djd.yj202588.top

C#:   // 自定义异常类中加 Code 属性
来源：http://erp.jinqigufen.top

[H10] 资源自动释放
来源：http://irh.svipenyu.cn

Py:   with open("a.txt") as f: data = f.read()
来源：http://mbw.ehwqpu.com

PHP:  // 无 with：在 finally 里 fclose()
来源：http://cgo.jianghu66.top

JS:   // 无 with：在 finally 里关闭句柄
来源：http://ham.cucudq.cn

TS:   // 无 with：在 finally 里关闭句柄
来源：http://srz.jinqigufen.top

Java: try (var in = new FileInputStream("a")) { }   // try-with-resources
来源：http://szu.cucudq.cn

Go:   defer f.Close()
来源：http://igx.wangshuangyany.cn

Ruby: File.open("a.txt") { |f| f.read }
来源：http://neb.yuanzhike.top

C#:   using var stream = File.OpenRead("a.txt");
来源：http://qwg.chenlongwang.top

================================================================================
来源：http://iwv.hnxiangtu.top

I. 正则表达式
来源：http://fce.guowangkeji.top

================================================================================
来源：http://ist.sjlbkw.cn

[I01] 判断是否匹配
来源：http://mgw.feifeiyinyue.top

Py:   re.search(r"\d+", s);  re.fullmatch(r"\d+", s)
来源：http://kss.jinyuanbaomall.cn

PHP:  preg_match('/\d+/', $s);
来源：http://nxa.ybcxt.top

JS:   /\d+/.test(s)
来源：http://hnf.pycfn.com

TS:   /\d+/.test(s)
来源：http://ywt.yj20258.top

Java: Pattern.compile("\\d+").matcher(s).find()
来源：http://iyz.chenzaomai.com

Go:   regexp.MustCompile(`\d+`).MatchString(s)
来源：http://edm.fehbvm.com

Ruby: s.match?(/\d+/)
来源：http://cri.hammf.cn

C#:   Regex.IsMatch(s, @"\d+")
来源：http://vod.zhengqikj.top

[I02] 提取所有匹配
来源：http://bsb.feifeiyinyue.top

Py:   re.findall(r"\d+", s)
来源：http://pgl.316326.xyz

PHP:  preg_match_all('/\d+/', $s, $m);  $m[0]
来源：http://huu.nwbrower.top

JS:   s.match(/\d+/g);  [...s.matchAll(/\d+/g)]
来源：http://csc.yj202588.top

TS:   s.match(/\d+/g)
来源：http://mtb.birdmap.top

Java: Pattern.compile("\\d+").matcher(s).results().toList()
来源：http://vpn.smart0.xyz

Go:   regexp.MustCompile(`\d+`).FindAllString(s, -1)
来源：http://hbz.andypj.xyz

Ruby: s.scan(/\d+/)
来源：http://bui.shuidangran.top

C#:   Regex.Matches(s, @"\d+").Select(m => m.Value).ToList()
来源：http://pii.fehbvm.com

[I03] 提取捕获分组
来源：http://rna.fzhhl.top

Py:   m = re.search(r"(\d+)-(\d+)", s);  m.group(1)
来源：http://sfq.sxryk.cn

PHP:  preg_match('/(\d+)-(\d+)/', $s, $m);  $m[1]
来源：http://njl.yj20258.top

JS:   const m = s.match(/(\d+)-(\d+)/);  m[1]
来源：http://anl.hongshengwenyu.top

TS:   const m = s.match(/(\d+)-(\d+)/);  m?.[1]
来源：http://wtg.aizwys.cn

Java: Matcher m = p.matcher(s);  if (m.find()) m.group(1);
来源：http://esy.xingfuxueyuan.xyz

Go:   m := re.FindStringSubmatch(s);  m[1]     // [0] 是整段
来源：http://ebj.zdbjq.cn

Ruby: s.match(/(\d+)-(\d+)/)[1]
来源：http://iwe.ppjwa.cn

C#:   Regex.Match(s, @"(\d+)-(\d+)").Groups[1].Value
来源：http://ovp.jqgfzy.top

[I04] 正则替换
来源：http://pfu.shangyingyoupin.top

Py:   re.sub(r"\d+", "#", s)
来源：http://bgj.hnxiangtu.top

PHP:  preg_replace('/\d+/', '#', $s);
来源：http://tdy.epnwcf.com

JS:   s.replace(/\d+/g, "#")
来源：http://vuw.tarul.cn

TS:   s.replace(/\d+/g, "#")
来源：http://zlh.kuanghao11.cn

Java: s.replaceAll("\\d+", "#")
来源：http://ebj.hysaishi.cn

Go:   re.ReplaceAllString(s, "#")
来源：http://njg.fengsongda.top

Ruby: s.gsub(/\d+/, "#")
来源：http://zhb.xylfe.cn

C#:   Regex.Replace(s, @"\d+", "#")
来源：http://skb.shuidangran.top

[I05] 按正则拆分
来源：http://prz.ehwqpu.com

Py:   re.split(r"\s*,\s*", s)
来源：http://feh.hywenlv.cn

PHP:  preg_split('/\s*,\s*/', $s);
来源：http://vpa.fehbvm.com

JS:   s.split(/\s*,\s*/)
来源：http://log.bjfxy.top

TS:   s.split(/\s*,\s*/)
来源：http://fok.yj20258888.top

Java: s.split("\\s*,\\s*")
来源：http://ebi.zhengqikj.top

Go:   regexp.MustCompile(`\s*,\s*`).Split(s, -1)
来源：http://fwm.yonumen.top

Ruby: s.split(/\s*,\s*/)
来源：http://qat.ivvv.top

C#:   Regex.Split(s, @"\s*,\s*")
来源：http://ktg.gzhubu.top

[I06] 常用校验模式（邮箱 / 手机号）
来源：http://qry.c1oappe.top

Py:   r"[^@]+@[^@]+\.[^@]+"；r"^1[3-9]\d{9}$"
来源：http://gog.zhixingplan.top

PHP:  '/^[^\s@]+@[^\s@]+\.[^\s@]+$/'；'/^1[3-9]\d{9}$/'
来源：http://uxw.hnxiangtu.top

JS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://vif.guowangkeji.top

TS:   /^[^\s@]+@[^\s@]+\.[^\s@]+$/；/^1[3-9]\d{9}$/
来源：http://nli.jianghu66.top

Java: "^[\\w.+-]+@[\\w-]+\\.[\\w.]+$"；"^1[3-9]\\d{9}$"
来源：http://mso.zhiwuduotai.top

Go:   `^[\w.+-]+@[\w-]+\.[\w.]+$`   // RE2 不支持反向引用与前瞻
来源：http://qgd.yj20258888.top

Ruby: /\A[\w.+-]+@[\w-]+\.[\w.]+\z/；/\A1[3-9]\d{9}\z/
来源：http://eql.hywenlv.cn

C#:   @"^[\w.+-]+@[\w-]+\.[\w.]+$"；@"^1[3-9]\d{9}$"
来源：http://xvk.jqgfzy.top

[I07] 忽略大小写与多行模式
来源：http://twq.sysykeji.top

Py:   re.findall(r"error", s, re.I | re.M)
来源：http://nyx.daria6918.cn

PHP:  preg_match_all('/error/im', $s, $m);
来源：http://uut.shanyushiyangkeji.top

JS:   /error/gim；new RegExp("error", "gim")
来源：http://nbo.pycfn.com

TS:   /error/gim
来源：http://hgu.birdmap.top

Java: Pattern.compile("error", Pattern.CASE_INSENSITIVE | Pattern.MULTILINE)
来源：http://mtb.havefunace.top

Go:   regexp.MustCompile(`(?im)error`)
来源：http://bqp.tanke756.top

Ruby: s.scan(/error/i)
来源：http://hso.hfpthk.cn

C#:   Regex.Match(s, "error", RegexOptions.IgnoreCase | RegexOptions.Multiline)
来源：http://lma.hesvh.cn

[I08] 贪婪与非贪婪匹配
来源：http://wjx.daxiang520.top

Py:   re.findall(r"<b>.*?</b>", s)       # 加 ? 变非贪婪
来源：http://pnf.hesvh.cn

PHP:  preg_match_all('/<b>.*?<\/b>/', $s, $m);
来源：http://fly.ivvv.top

JS:   s.match(/<b>.*?<\/b>/g)
来源：http://irr.xuanzx.com

TS:   s.match(/<b>.*?<\/b>/g)
来源：http://jqd.ehwqpu.com

Java: Pattern.compile("<b>.*?</b>")
来源：http://wge.chenjidiqi.icu

Go:   `<b>.*?</b>`                      # RE2 默认贪婪，同样用 ? 抑制
来源：http://vdb.dianchejie.cn

Ruby: s.scan(/<b>.*?<\/b>/)
来源：http://vyt.jinqigfzy.top

C#:   Regex.Matches(s, @"<b>.*?</b>")
来源：http://vow.jinyuanbaomall.cn

================================================================================
来源：http://quu.tarul.cn

J. 日期与时间
来源：http://iil.jinqigufen.top

================================================================================
来源：http://kkj.fehbvm.com

[J01] 获取当前时间
来源：http://lam.fengsongda.top

Py:   datetime.now();  datetime.now(UTC)
来源：http://xuu.zhijiandao.cn

PHP:  new DateTimeImmutable();  date("Y-m-d H:i:s");
来源：http://sjq.feifeiyinyue.top

JS:   new Date();  Date.now()
来源：http://juq.daria6918.cn

TS:   new Date();  Date.now()
来源：http://abq.gzhubu.top

Java: LocalDateTime.now();  Instant.now()
来源：http://bpj.ehwqpu.com

Go:   time.Now()
来源：http://wna.havefunace.top

Ruby: Time.now
来源：http://orf.hnqzz.top

C#:   DateTime.Now;  DateTime.UtcNow
来源：http://mwa.quarkkingdee.top

[J02] 格式化输出
来源：http://blq.fktsv.cn

Py:   now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://quz.jyoumei.cn

PHP:  (new DateTime())->format("Y-m-d H:i:s");
来源：http://els.yongpay.top

JS:   d.toISOString();  d.toLocaleString("zh-CN")
来源：http://gjq.zhoulong.xyz

TS:   d.toISOString()
来源：http://ssi.hnxiangtu.top

Java: DateTimeFormatter.ofPattern("yyyy-MM-dd HH:mm:ss").format(LocalDateTime.now())
来源：http://gpy.zycfv.cn

Go:   time.Now().Format("2006-01-02 15:04:05")     // Go 用参考时间做格式
来源：http://fbl.fengsongda.top

Ruby: Time.now.strftime("%Y-%m-%d %H:%M:%S")
来源：http://lye.cheryme.top

C#:   DateTime.Now.ToString("yyyy-MM-dd HH:mm:ss")
来源：http://zta.ywan-chungtsiang.top

[J03] 字符串解析为日期
来源：http://wia.sxryk.cn

Py:   datetime.strptime("2024-01-02", "%Y-%m-%d")
来源：http://pkj.yanxiufei.cn

PHP:  DateTimeImmutable::createFromFormat("Y-m-d", "2024-01-02");
来源：http://znn.dianchejie.cn

JS:   new Date("2024-01-02")
来源：http://mag.sjlbkw.cn

TS:   new Date("2024-01-02")
来源：http://yfv.vehdjk.com

Java: LocalDate.parse("2024-01-02")
来源：http://lza.jianghu66.top

Go:   time.Parse("2006-01-02", "2024-01-02")
来源：http://ykm.zhaomingkeji.xyz

Ruby: Date.parse("2024-01-02")
来源：http://hxz.zhongyouzk.top

C#:   DateTime.Parse("2024-01-02");  DateTime.ParseExact("2024-01-02", "yyyy-MM-dd", null)
来源：http://nhx.zhiwuduotai.top

[J04] 时间戳与日期互转
来源：http://wvv.jinyuanbaomall.cn

Py:   int(now.timestamp());  datetime.fromtimestamp(ts)
来源：http://acd.hysaishi.cn

PHP:  time();  (new DateTime())->getTimestamp();
来源：http://ffo.hnqzz.top

JS:   Math.floor(Date.now() / 1000);  new Date(ts * 1000)
来源：http://ajl.yuanzhike.top

TS:   Math.floor(Date.now() / 1000)
来源：http://xvt.vehdjk.com

Java: Instant.now().getEpochSecond();  Instant.ofEpochSecond(ts)
来源：http://rne.pycfn.com

Go:   time.Now().Unix();  time.Unix(ts, 0)
来源：http://pfr.zhijiandao.cn

Ruby: Time.now.to_i;  Time.at(ts)
来源：http://rvx.birdmap.top

C#:   DateTimeOffset.UtcNow.ToUnixTimeSeconds();  DateTimeOffset.FromUnixTimeSeconds(ts)
来源：http://piy.sjlbkw.cn

[J05] 时间加减（加 7 天）
来源：http://wrn.yuanzhike.top

Py:   now + timedelta(days=7)
来源：http://jyf.hfpthk.cn

PHP:  (new DateTime())->modify("+7 days");
来源：http://pqa.pycfn.com

JS:   new Date(Date.now() + 7 * 86400000)
来源：http://nno.jlsjyb.cn

TS:   new Date(Date.now() + 7 * 86400000)
来源：http://gej.shangyingyoupin.top

Java: LocalDate.now().plusDays(7)
来源：http://wyi.cqqwz.cn

Go:   time.Now().AddDate(0, 0, 7)
来源：http://uev.feifeiyinyue.top

Ruby: Time.now + 7 * 86400
来源：http://mtc.jqgfzy.top

C#:   DateTime.Now.AddDays(7)
来源：http://dey.yongpay.top

[J06] 计算两时间之差
来源：http://hup.wangshuangyany.cn

Py:   (end - start).total_seconds()
来源：http://cdj.zhoulong.xyz

PHP:  $end->diff($start)->days;
来源：http://rdi.hongshengwenyu.top

JS:   (end - start) / 1000        // 毫秒差转秒
来源：http://zwf.dashuyun.cn

TS:   (end.getTime() - start.getTime()) / 1000
来源：http://dvi.guannengcc.top

Java: Duration.between(start, end).toSeconds()
来源：http://nwd.shzxlz.cn

Go:   end.Sub(start).Hours()
来源：http://nur.jinqigfzy.top

Ruby: end - start                 # 返回秒数
来源：http://rtx.aibaodan.cn

C#:   (end - start).TotalSeconds
来源：http://cze.cdnleiting.top

[J07] 比较两个日期
来源：http://bpw.haohaochexian.top

Py:   d1 < d2;  d1 == d2
来源：http://cfi.hesvh.cn

PHP:  $d1 < $d2;  $d1 == $d2;
来源：http://frc.pengpengdd.cyou

JS:   d1.getTime() < d2.getTime()
来源：http://zpj.yfazqb.com

TS:   d1.getTime() < d2.getTime()
来源：http://zgh.cqqwz.cn

Java: d1.isBefore(d2);  d1.isEqual(d2)
来源：http://oeg.smart0.xyz

Go:   d1.Before(d2);  d1.Equal(d2)
来源：http://dsw.ctjpmb.com

Ruby: d1 < d2;  d1 == d2
来源：http://fxr.hfpthk.cn

C#:   d1 < d2;  d1 == d2
来源：http://aff.xinyue.icu

[J08] 提取年月日与星期
来源：http://tgd.xinyue.icu

Py:   d.year;  d.month;  d.day;  d.weekday()
来源：http://hqv.sxryk.cn

PHP:  (int) date("Y");  (int) date("n");  (int) date("j");  (int) date("w");
来源：http://ivl.uphjek.com


<!-- 参考信息 -->