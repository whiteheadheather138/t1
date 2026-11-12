代发 wailian999

[Q78] 当前时间
来源：http://iqy.aibaodan.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://nus.ydjk.org.cn

[Q79] 字符串拼接
来源：http://oly.cheryme.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://ueh.mhx1999.top

[Q80] 字符串截取
来源：http://dny.cashguo.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://gwj.yj20258.top

[Q81] 字符串替换
来源：http://fhs.hesvh.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://owf.gotoacloud.top

[Q82] 字符长度与字节长度
来源：http://iui.pycfn.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://kwi.epnwcf.com

[Q83] 大小写转换
来源：http://rqw.hysaishi.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://uvw.ybcxt.top

[Q84] 去除首尾空格
来源：http://szo.xingfuxueyuan.xyz

SELECT TRIM(name) FROM users;
来源：http://edz.wangshuangyany.cn

[Q85] 数值取整
来源：http://oug.nanxuanxn.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://nsj.xylfe.cn

[Q86] 读取 JSON 字段
来源：http://qdt.316326.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://onr.jlsjyb.cn

[Q87] JSON 字段做条件
来源：http://zmd.meibo888.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://fsi.52xcode.cn

[Q88] 行转列（条件聚合）
来源：http://ptl.zhongyouzk.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://oih.316326.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://txn.zycfv.cn

[Q89] 判断表是否存在
来源：http://wyi.zhijiandao.cn

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vjp.epnwcf.com

[Q90] 生成序号列
来源：http://opo.quarkkingdee.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://yxp.cqqwz.cn

================================================================================
来源：http://ddc.pycfn.com

R. Bash 专题
来源：http://vuq.zhoulong.xyz

================================================================================
来源：http://sjc.sxryk.cn

[R01] shebang 与严格模式
来源：http://vro.kuanghao11.cn

#!/usr/bin/env bash
来源：http://ejj.wangdashe.top

set -euo pipefail
来源：http://iva.ybcxt.top

[R02] 变量赋值与使用
来源：http://bpj.yuanzhike.top

name="Tom"; echo "$name"
来源：http://bwf.chenjidiqi.icu

[R03] 只读变量
来源：http://xkg.kuanghao11.cn

readonly PI=3.14
来源：http://tfb.tarul.cn

[R04] 位置参数
来源：http://pip.xylfe.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://krm.nanxinkj.top

[R05] 参数默认值
来源：http://xqd.vqdsnc.cn

name="${1:-default}"
来源：http://fyk.jqgufenzy.top

[R06] 判断命令是否存在
来源：http://kly.xylfe.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wlw.haohaochexian.top

[R07] if 判断文件
来源：http://xhx.shzxlz.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://aav.svipenyu.cn

[R08] 数值比较
来源：http://tut.ybcxt.top

if (( a > b )); then echo "a 更大"; fi
来源：http://qbp.aibaodan.cn

[R09] 字符串比较
来源：http://nva.tanke756.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://bvc.ywan-chungtsiang.top

[R10] 正则匹配
来源：http://kpu.yangfankeji.com

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://nqq.smart0.xyz

[R11] case 多分支
来源：http://uqz.yvedp.cn

case "$1" in
来源：http://tpd.ctjpmb.com

start) echo "启动" ;;
来源：http://xgi.dianchejie.cn

stop)  echo "停止" ;;
来源：http://qgk.cucudq.cn

*)     echo "未知命令" ;;
来源：http://alg.xziqi.cn

esac
来源：http://pys.jinghuilouyu.cn

[R12] for 遍历文件
来源：http://sze.wangshuangyany.cn

for f in *.txt; do echo "$f"; done
来源：http://zhu.hnxiangtu.top

[R13] for 计数循环
来源：http://ckx.xuanzx.com

for i in {1..10}; do echo "$i"; done
来源：http://oas.fktsv.cn

[R14] C 风格 for
来源：http://svh.tianlin.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wvy.tarul.cn

[R15] while 逐行读文件
来源：http://kvc.hongshengwenyu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://lsj.smart0.xyz

[R16] until 等待条件
来源：http://jqm.316326.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://chg.guannengcc.top

[R17] 数组定义与取值
来源：http://bwu.yangfankeji.com

arr=(a b c); echo "${arr[0]}"
来源：http://jbs.epnwcf.com

[R18] 遍历数组
来源：http://kif.chenzaomai.com

for x in "${arr[@]}"; do echo "$x"; done
来源：http://ujd.yuanzhike.top

[R19] 数组长度
来源：http://fys.nanxinkj.top

echo "${#arr[@]}"
来源：http://vhu.nanxuanxn.top

[R20] 关联数组（字典）
来源：http://njj.hnqzz.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xij.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://cos.fengsongda.top

echo "${#s}"
来源：http://iqm.mhx1999.top

[R22] 截取子串
来源：http://zqk.zhongyouzk.top

echo "${s:0:5}"
来源：http://rof.yueranfly.top

[R23] 字符串替换
来源：http://ywx.ctjpmb.com

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fuk.tian-w.cn

[R24] 大小写转换
来源：http://hov.hammf.cn

echo "${s^^}"; echo "${s,,}"
来源：http://yvi.nanxinkj.top

[R25] 去后缀 / 去前缀
来源：http://frv.cdnleiting.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://utl.bjfxy.top

[R26] 命令替换
来源：http://qst.hcnkem.com

now=$(date +%F); echo "$now"
来源：http://rcz.bjfxy.top

[R27] 算术展开
来源：http://idj.yongpay.top

echo $((1 + 2 * 3))
来源：http://zci.zhengqikj.top

[R28] 浮点运算
来源：http://cgs.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://inz.wangdashe.top

[R29] 定义函数
来源：http://her.snrcjt.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mnl.pycfn.com

[R30] 函数返回状态码
来源：http://aoq.shangyingyoupin.top

f() { return 0; }; f || echo "失败了"
来源：http://puc.fktsv.cn

[R31] 局部变量
来源：http://wjo.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://cgv.ivvv.top

[R32] 参数个数校验
来源：http://reo.birdmap.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://tbn.zycfv.cn

[R33] 捕获错误并提示行号
来源：http://hts.ybcxt.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://ihs.cqqwz.cn

[R34] 退出时清理
来源：http://jhp.jinyuanbaomall.cn

trap 'rm -f "$tmp"' EXIT
来源：http://ehk.vqdsnc.cn

[R35] 后台执行并等待
来源：http://zxx.nanxuanxn.top

sleep 5 & pid=$!; wait "$pid"
来源：http://hml.chenjidiqi.icu

[R36] 并发执行多个任务
来源：http://kvf.hysaishi.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://zyq.aizwys.cn

[R37] 把输出赋给变量
来源：http://dll.gaohongyu789.top

files=$(ls -1)
来源：http://aih.meibo888.top

[R38] 管道串联
来源：http://krn.fehbvm.com

cat a.txt | grep -i error | wc -l
来源：http://dlv.nanxuanxn.top

[R39] 重定向标准输出与错误
来源：http://vrk.wangdashe.top

cmd > out.log 2>&1
来源：http://lzx.zdqjudy.top

[R40] 追加写日志
来源：http://mlk.chenlongwang.top

echo "log" >> out.log
来源：http://uqe.ivvv.top

[R41] 丢弃输出
来源：http://fjn.jiagoushi.top

cmd >/dev/null 2>&1
来源：http://xkx.yuxming.cn

[R42] 输入重定向
来源：http://omd.nanxuanxn.top

wc -l < a.txt
来源：http://nep.0kj1m.cn

[R43] 按名字查找文件
来源：http://nyq.nanxuanxn.top

find . -name "*.log" -type f
来源：http://bwu.zhixingplan.top

[R44] 按修改时间查找
来源：http://gml.tarul.cn

find . -mtime -7 -type f
来源：http://oyz.hongshengwenyu.top

[R45] 批量删除
来源：http://dfn.daxiang520.top

find . -name "*.tmp" -delete
来源：http://eks.hnxiangtu.top

[R46] 递归替换文件内容
来源：http://bhs.yuanzhike.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://flo.jianghu66.top

[R47] sed 单行替换
来源：http://vlt.jqgufenzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://cnb.daria6918.cn

[R48] awk 取指定列
来源：http://ogy.jqgfzy.top

awk '{print $1, $3}' a.txt
来源：http://ysq.cdnleiting.top

[R49] awk 带条件
来源：http://nqn.nwbrower.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://fup.iojbl.cn

[R50] awk 求和
来源：http://nfy.yfazqb.com

awk '{s += $2} END {print s}' a.txt
来源：http://uca.daxiang520.top

[R51] 排序去重取前几
来源：http://kwy.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xch.jianghu66.top

[R52] 统计行数
来源：http://nab.shzxlz.cn

wc -l a.txt
来源：http://pdj.hammf.cn

[R53] 查看文件头与实时尾
来源：http://edc.fehbvm.com

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ihw.zhoulong.xyz

[R54] 比较两个文件
来源：http://cck.andypj.xyz

diff a.txt b.txt
来源：http://yrd.jinghuilouyu.cn

[R55] 压缩与解压
来源：http://yfa.fengsongda.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://nhw.redwolf501.top

[R56] 远程拷贝
来源：http://qhg.hnqzz.top

scp file user@host:/path/
来源：http://vpq.ybcxt.top

[R57] 远程执行命令
来源：http://gev.bbcook.cn

ssh user@host 'uptime'
来源：http://mgj.ydjk.org.cn

[R58] 下载文件
来源：http://pmd.cqqwz.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bfd.daxiang520.top

[R59] 发 POST JSON
来源：http://jgw.chenzaomai.com

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zhj.nanxinkj.top

[R60] 只看 HTTP 状态码
来源：http://zzw.pengpengdd.cyou

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pli.fanxiaobao.xyz

[R61] 磁盘占用
来源：http://imn.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://uiz.aibaodan.cn

[R62] 找最占空间的文件
来源：http://jyt.cdnleiting.top

du -ah . | sort -rh | head -10
来源：http://giy.ywan-chungtsiang.top

[R63] 内存与进程
来源：http://vvj.dianchejie.cn

free -h;  ps aux | grep nginx
来源：http://ksu.uphjek.com

[R64] 结束进程
来源：http://clo.zhaomingkeji.xyz

kill -9 $(pgrep -f app.py)
来源：http://avt.xinyue.icu

[R65] 查看端口占用
来源：http://wyr.xinyue.icu

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kjg.tianlin.xyz

[R66] 定时任务
来源：http://gkb.uphjek.com

crontab -e;  crontab -l
来源：http://ncq.ctjpmb.com

[R67] 生成随机十六进制串
来源：http://bqw.feifeiyinyue.top

openssl rand -hex 16
来源：http://hzj.zhoulong.xyz

[R68] 计算文件校验值
来源：http://ptu.fktsv.cn

sha256sum a.txt;  md5sum a.txt
来源：http://geo.yonumen.top

[R69] 生成随机密码
来源：http://jdd.zdqjudy.top

head -c 16 /dev/urandom | base64
来源：http://vnz.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://hcr.jiagoushi.top

date +%s;  date -d @1700000000
来源：http://sfs.havefunace.top

[R71] 日期格式化
来源：http://ecc.sufxvd.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lqa.birdmap.top

[R72] 等待端口就绪
来源：http://qip.feifeiyinyue.top

until nc -z localhost 3306; do sleep 1; done
来源：http://rhc.tianlin.xyz

[R73] 分割大日志
来源：http://ort.feifeiyinyue.top

split -l 1000 big.log part_
来源：http://iqj.yvedp.cn

[R74] 批量重命名
来源：http://msi.gotoacloud.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xbz.uphjek.com

[R75] 导出环境变量
来源：http://nhz.pengpengdd.cyou

export PATH="$HOME/bin:$PATH"
来源：http://wkd.yuxming.cn

[R76] 使用临时文件
来源：http://pnq.yanxiufei.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gir.mhx1999.top

[R77] 读取用户输入
来源：http://gtw.xziqi.cn

read -rp "请输入: " ans
来源：http://nyr.wangshuangyany.cn

[R78] 交互式菜单
来源：http://urp.sjlbkw.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wme.zhixingplan.top

[R79] 解析命令行选项
来源：http://vjm.yanxiufei.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rqj.nanxuanxn.top

[R80] 查看脚本执行耗时
来源：http://gci.hnqzz.top

time ./run.sh
来源：http://sbr.hnqzz.top

================================================================================
来源：http://hgx.uphjek.com

S. C / C++ 专题
来源：http://ojc.cqqwz.cn

================================================================================
来源：http://gec.zhongyouzk.top

[S01] C：Hello World
来源：http://xms.tian-w.cn

#include <stdio.h>
来源：http://mxf.aibaodan.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qtw.zhiwuduotai.top

[S02] C：变量与格式化输出
来源：http://cpo.uphjek.com

int a = 10; printf("%d\n", a);
来源：http://ejw.xinyue.icu

[S03] C：读入整数
来源：http://tpq.gaohongyu789.top

int x; scanf("%d", &x);
来源：http://mua.xinyue.icu

[S04] C：字符串复制
来源：http://lqv.zycfv.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fjv.xuetiantiany.cn

[S05] C：字符串长度
来源：http://oro.yj20258.top

strlen(s)
来源：http://cyz.wangshuangyany.cn

[S06] C：字符串比较
来源：http://vob.hongshengwenyu.top

strcmp(a, b) == 0
来源：http://gmc.hammf.cn

[S07] C：数组遍历求和
来源：http://qbx.xylfe.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zzj.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://yyr.jinghuilouyu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tlg.ybcxt.top

[S09] C：结构体定义与初始化
来源：http://mgl.yangfankeji.com

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ywt.tarul.cn

[S10] C：指针与解引用
来源：http://qgx.sufxvd.cn

int *p = &a;  *p = 5;
来源：http://xpl.fanxiaobao.xyz

[S11] C：逐行读文件
来源：http://mvj.guowangkeji.top

FILE *f = fopen("a.txt", "r");
来源：http://are.xuanzx.com

while (fgets(buf, sizeof buf, f)) { }
来源：http://efa.zdqjudy.top

fclose(f);
来源：http://cao.ppjwa.cn

[S12] C：写文件
来源：http://rlx.dianchejie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://luf.shangyingyoupin.top

[S13] C：宏定义
来源：http://hya.jiagoushi.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vcy.cdnleiting.top

[S14] C：枚举
来源：http://jqh.chenjidiqi.icu

enum Color { RED, GREEN, BLUE };
来源：http://yfv.yfazqb.com

[S15] C：类型转换
来源：http://sxf.gzhubu.top

(double) a / b
来源：http://inp.jqgufenzy.top

[S16] C：位操作置位
来源：http://ige.gzhubu.top

x |= (1 << 3);
来源：http://wen.fzhhl.top

[S17] C：安全拼接字符串
来源：http://ftp.bjfxy.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://prk.ehwqpu.com

[S18] C：命令行参数
来源：http://lsf.gzhubu.top

int main(int argc, char **argv)
来源：http://npv.52xcode.cn

[S19] C：快速排序
来源：http://nqc.chenlongwang.top

qsort(a, n, sizeof(int), cmp);
来源：http://vyw.fzhhl.top

[S20] C：二分查找
来源：http://gxf.snrcjt.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fjy.fktsv.cn

[S21] C：字符类别判断
来源：http://iar.zhijiandao.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://usa.fengsongda.top

[S22] C：字符串转数字
来源：http://ins.zhengqikj.top

atoi("42");  strtod("3.14", NULL);
来源：http://rob.xinyue.icu

[S23] C：随机数
来源：http://awq.316326.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://pwi.cashguo.top

[S24] C：获取本地时间
来源：http://cti.ydzc1.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dfm.cqqwz.cn

[S25] C：内存拷贝
来源：http://wfo.daxiang520.top

memcpy(dst, src, n);
来源：http://lcx.yonumen.top

[S26] C：内存清零
来源：http://pdo.jinqigufen.top

memset(a, 0, sizeof a);
来源：http://fyo.cdnleiting.top

[S27] C：定义常量
来源：http://ydh.birdmap.top

const double PI = 3.14159;
来源：http://nwj.nwbrower.top

[S28] C：静态变量
来源：http://juf.iojbl.cn

static int counter = 0;
来源：http://eqa.ydjk.org.cn

[S29] C：变参函数
来源：http://rtk.quarkkingdee.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xuz.yuanzhike.top

[S30] C：头文件保护
来源：http://fzz.zhixingplan.top

#ifndef X_H
来源：http://xsz.quarkkingdee.top

#define X_H
来源：http://yws.aibaodan.cn

#endif
来源：http://pfm.jlsjyb.cn

[S31] C++：Hello World
来源：http://ssp.shangyingyoupin.top

#include <iostream>
来源：http://euw.nanxinkj.top

int main() { std::cout << "Hello\n"; }
来源：http://ygr.jianghu66.top

[S32] C++：字符串
来源：http://ehj.gotoacloud.top

std::string s = "hi";  s += "!";
来源：http://mdv.iojbl.cn

[S33] C++：vector 增删
来源：http://ldk.aibaodan.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xtt.wangdashe.top

[S34] C++：遍历 vector
来源：http://wkn.zhongyouzk.top

for (auto &x : v) { std::cout << x; }
来源：http://oab.zhijiandao.cn

[S35] C++：map
来源：http://kwh.aizwys.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dpw.jianghu66.top

[S36] C++：unordered_map
来源：http://etc.ywan-chungtsiang.top

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vlf.yangfankeji.com

[S37] C++：set
来源：http://ook.xingfuxueyuan.xyz

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mgz.ctjpmb.com

[S38] C++：排序
来源：http://mbv.bbcook.cn

std::sort(v.begin(), v.end());
来源：http://snz.shuidangran.top

[S39] C++：自定义比较器排序
来源：http://zwd.ywan-chungtsiang.top

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lhf.quarkkingdee.top

[S40] C++：查找元素
来源：http://ecn.yuxming.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hvv.gogol.net.cn

[S41] C++：类与构造函数
来源：http://lci.ctjpmb.com

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lxj.pengpengdd.cyou

[S42] C++：继承与虚函数
来源：http://vud.yvedp.cn

class B : public Base { public: void f() override {} };
来源：http://rkk.hnxiangtu.top

[S43] C++：智能指针
来源：http://exv.xziqi.cn

auto p = std::make_unique<int>(5);
来源：http://jfo.yj20258.top

[S44] C++：引用传参
来源：http://snp.uphjek.com

void inc(int &x) { ++x; }
来源：http://ymb.xingfuxueyuan.xyz

[S45] C++：lambda
来源：http://bva.xinyue.icu

auto add = [](int a, int b) { return a + b; };
来源：http://nkl.uphjek.com

[S46] C++：函数模板
来源：http://gpr.birdmap.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fdk.shzxlz.cn

[S47] C++：结构化绑定遍历
来源：http://umi.mhx1999.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://eou.pycfn.com

[S48] C++：逐行读文件
来源：http://qrt.daxiang520.top

std::ifstream in("a.txt");  std::string line;
来源：http://hhj.nanxinkj.top


<!-- 参考信息 -->