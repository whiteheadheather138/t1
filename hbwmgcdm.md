代发 wailian999

[Q78] 当前时间
来源：http://aui.xylfe.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://lfm.tarul.cn

[Q79] 字符串拼接
来源：http://key.jiagoushi.top

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://zhu.hcnkem.com

[Q80] 字符串截取
来源：http://mgq.havefunace.top

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://iuz.ivvv.top

[Q81] 字符串替换
来源：http://nvn.wangdashe.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mcl.jlsjyb.cn

[Q82] 字符长度与字节长度
来源：http://qzz.haohaochexian.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://hbx.9152youxi.cn

[Q83] 大小写转换
来源：http://nod.guowangkeji.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://fpz.cashguo.top

[Q84] 去除首尾空格
来源：http://owa.zhijiandao.cn

SELECT TRIM(name) FROM users;
来源：http://wcd.dashuyun.cn

[Q85] 数值取整
来源：http://suf.wangdashe.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wjf.uphjek.com

[Q86] 读取 JSON 字段
来源：http://vwi.ehwqpu.com

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://xfe.jqgfzy.top

[Q87] JSON 字段做条件
来源：http://bqg.havefunace.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://uzs.vqdsnc.cn

[Q88] 行转列（条件聚合）
来源：http://jgr.hammf.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://fxk.ywan-chungtsiang.top

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://tra.cashguo.top

[Q89] 判断表是否存在
来源：http://eks.yueranfly.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://xew.yanxiufei.cn

[Q90] 生成序号列
来源：http://oca.hnqzz.top

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xdv.wangshuangyany.cn

================================================================================
来源：http://nsu.quarkkingdee.top

R. Bash 专题
来源：http://gwu.jlsjyb.cn

================================================================================
来源：http://hhc.hfpthk.cn

[R01] shebang 与严格模式
来源：http://oeb.gogol.net.cn

#!/usr/bin/env bash
来源：http://nbz.yuanzhike.top

set -euo pipefail
来源：http://dqw.gogol.net.cn

[R02] 变量赋值与使用
来源：http://aed.yuanzhike.top

name="Tom"; echo "$name"
来源：http://pyy.fktsv.cn

[R03] 只读变量
来源：http://yvj.meibo888.top

readonly PI=3.14
来源：http://hwq.jinqigfzy.top

[R04] 位置参数
来源：http://ncy.ydzc1.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://puy.316326.xyz

[R05] 参数默认值
来源：http://fym.sjlbkw.cn

name="${1:-default}"
来源：http://qpr.aizwys.cn

[R06] 判断命令是否存在
来源：http://puh.hnqzz.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ndq.shangyingyoupin.top

[R07] if 判断文件
来源：http://smc.jiagoushi.top

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://bry.aibaodan.cn

[R08] 数值比较
来源：http://lnb.hongshengwenyu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ksi.guowangkeji.top

[R09] 字符串比较
来源：http://pbp.sysykeji.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://zds.hesvh.cn

[R10] 正则匹配
来源：http://gpd.iojbl.cn

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://lje.hcnkem.com

[R11] case 多分支
来源：http://kow.ppjwa.cn

case "$1" in
来源：http://xms.dianchejie.cn

start) echo "启动" ;;
来源：http://ija.ivvv.top

stop)  echo "停止" ;;
来源：http://xlh.haohaochexian.top

*)     echo "未知命令" ;;
来源：http://pxs.zhaomingkeji.xyz

esac
来源：http://ecl.ehwqpu.com

[R12] for 遍历文件
来源：http://flk.daxiang520.top

for f in *.txt; do echo "$f"; done
来源：http://bfc.epnwcf.com

[R13] for 计数循环
来源：http://jqk.mhx1999.top

for i in {1..10}; do echo "$i"; done
来源：http://rva.zhaomingkeji.xyz

[R14] C 风格 for
来源：http://sfm.zycfv.cn

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://jgj.haohaochexian.top

[R15] while 逐行读文件
来源：http://dah.gaohongyu789.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://vfq.vqdsnc.cn

[R16] until 等待条件
来源：http://yia.hywenlv.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://icm.vehdjk.com

[R17] 数组定义与取值
来源：http://vfc.yuxming.cn

arr=(a b c); echo "${arr[0]}"
来源：http://vui.zycfv.cn

[R18] 遍历数组
来源：http://nua.c1oappe.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://sks.yonumen.top

[R19] 数组长度
来源：http://bvv.redwolf501.top

echo "${#arr[@]}"
来源：http://rei.wangdashe.top

[R20] 关联数组（字典）
来源：http://wrd.haohaochexian.top

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://jhq.zhiwuduotai.top

[R21] 字符串长度
来源：http://ngu.yonumen.top

echo "${#s}"
来源：http://llt.gzhubu.top

[R22] 截取子串
来源：http://pml.pycfn.com

echo "${s:0:5}"
来源：http://pkl.yj202588.top

[R23] 字符串替换
来源：http://rbg.hnxiangtu.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://exa.andypj.xyz

[R24] 大小写转换
来源：http://vpf.tian-w.cn

echo "${s^^}"; echo "${s,,}"
来源：http://nox.zhiwuduotai.top

[R25] 去后缀 / 去前缀
来源：http://zbv.nwbrower.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://lsv.guannengcc.top

[R26] 命令替换
来源：http://krs.9152youxi.cn

now=$(date +%F); echo "$now"
来源：http://usy.jqgfzy.top

[R27] 算术展开
来源：http://emp.zhengqikj.top

echo $((1 + 2 * 3))
来源：http://qxh.vehdjk.com

[R28] 浮点运算
来源：http://cat.aibaodan.cn

echo "scale=2; 10/3" | bc
来源：http://hfd.yuxming.cn

[R29] 定义函数
来源：http://xjx.shzxlz.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://ovs.fehbvm.com

[R30] 函数返回状态码
来源：http://ang.hnxiangtu.top

f() { return 0; }; f || echo "失败了"
来源：http://uml.shanyushiyangtech.top

[R31] 局部变量
来源：http://eli.zhixingplan.top

f() { local x=1; echo "$x"; }
来源：http://wcn.jinyuanbaomall.cn

[R32] 参数个数校验
来源：http://jst.yj202588.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wwq.hysaishi.cn

[R33] 捕获错误并提示行号
来源：http://nsb.guannengcc.top

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://bpl.tarul.cn

[R34] 退出时清理
来源：http://sea.shanyushiyangtech.top

trap 'rm -f "$tmp"' EXIT
来源：http://soo.tian-w.cn

[R35] 后台执行并等待
来源：http://hmu.yj20258.top

sleep 5 & pid=$!; wait "$pid"
来源：http://jfr.zhixingplan.top

[R36] 并发执行多个任务
来源：http://lja.vqdsnc.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://msx.yj20258.top

[R37] 把输出赋给变量
来源：http://wwy.wangshuangyany.cn

files=$(ls -1)
来源：http://nwd.sysykeji.top

[R38] 管道串联
来源：http://ybj.52xcode.cn

cat a.txt | grep -i error | wc -l
来源：http://pih.jianghu66.top

[R39] 重定向标准输出与错误
来源：http://tze.xinyue.icu

cmd > out.log 2>&1
来源：http://zxq.yonumen.top

[R40] 追加写日志
来源：http://hsv.guannengcc.top

echo "log" >> out.log
来源：http://uel.fehbvm.com

[R41] 丢弃输出
来源：http://uxl.snrcjt.cn

cmd >/dev/null 2>&1
来源：http://szs.c1oappe.top

[R42] 输入重定向
来源：http://cci.pycfn.com

wc -l < a.txt
来源：http://jib.jiagoushi.top

[R43] 按名字查找文件
来源：http://hek.guowangkeji.top

find . -name "*.log" -type f
来源：http://kor.hysaishi.cn

[R44] 按修改时间查找
来源：http://gxm.mhx1999.top

find . -mtime -7 -type f
来源：http://ohb.chenzaomai.com

[R45] 批量删除
来源：http://zmd.tianlin.xyz

find . -name "*.tmp" -delete
来源：http://uas.zhiwuduotai.top

[R46] 递归替换文件内容
来源：http://srs.quarkkingdee.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ywv.iojbl.cn

[R47] sed 单行替换
来源：http://xqc.jinqigfzy.top

sed -i 's/foo/bar/g' a.txt
来源：http://vhh.daria6918.cn

[R48] awk 取指定列
来源：http://ucp.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://kiz.bbcook.cn

[R49] awk 带条件
来源：http://npe.gogol.net.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://are.shzxlz.cn

[R50] awk 求和
来源：http://crl.tanke756.top

awk '{s += $2} END {print s}' a.txt
来源：http://zaj.feifeiyinyue.top

[R51] 排序去重取前几
来源：http://prc.shanyushiyangtech.top

sort a.txt | uniq -c | sort -rn | head
来源：http://upp.zdbjq.cn

[R52] 统计行数
来源：http://qpc.yuxming.cn

wc -l a.txt
来源：http://nym.chenlongwang.top

[R53] 查看文件头与实时尾
来源：http://eze.aibaodan.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iiy.fengsongda.top

[R54] 比较两个文件
来源：http://cha.yvedp.cn

diff a.txt b.txt
来源：http://siy.ivvv.top

[R55] 压缩与解压
来源：http://zkv.nanxuanxn.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://fuj.yj202588.top

[R56] 远程拷贝
来源：http://bli.aibaodan.cn

scp file user@host:/path/
来源：http://ppj.andypj.xyz

[R57] 远程执行命令
来源：http://yxi.gotoacloud.top

ssh user@host 'uptime'
来源：http://eiy.jinyuanbaomall.cn

[R58] 下载文件
来源：http://acm.jiagoushi.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hjc.jinyuanbaomall.cn

[R59] 发 POST JSON
来源：http://vgo.yonumen.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kfz.fengsongda.top

[R60] 只看 HTTP 状态码
来源：http://znr.shanyushiyangtech.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nba.yj20258.top

[R61] 磁盘占用
来源：http://gri.xingfuxueyuan.xyz

df -h;  du -sh *
来源：http://zqw.ybcxt.top

[R62] 找最占空间的文件
来源：http://puq.shanyushiyangkeji.top

du -ah . | sort -rh | head -10
来源：http://zur.ybcxt.top

[R63] 内存与进程
来源：http://ufu.zycfv.cn

free -h;  ps aux | grep nginx
来源：http://jqy.yvedp.cn

[R64] 结束进程
来源：http://lwf.sjlbkw.cn

kill -9 $(pgrep -f app.py)
来源：http://gqz.zhengqikj.top

[R65] 查看端口占用
来源：http://vsv.xuanzx.com

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kxi.ywan-chungtsiang.top

[R66] 定时任务
来源：http://dwq.zhaomingkeji.xyz

crontab -e;  crontab -l
来源：http://myy.svipenyu.cn

[R67] 生成随机十六进制串
来源：http://vzv.nwbrower.top

openssl rand -hex 16
来源：http://ysy.xylfe.cn

[R68] 计算文件校验值
来源：http://srn.snrcjt.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ogc.fktsv.cn

[R69] 生成随机密码
来源：http://bbn.feifeiyinyue.top

head -c 16 /dev/urandom | base64
来源：http://fuh.smart0.xyz

[R70] 时间戳与互转
来源：http://wvs.sjlbkw.cn

date +%s;  date -d @1700000000
来源：http://yvu.xylfe.cn

[R71] 日期格式化
来源：http://qgf.yonumen.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://dnd.fanxiaobao.xyz

[R72] 等待端口就绪
来源：http://bkc.gogol.net.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://eyu.kuanghao11.cn

[R73] 分割大日志
来源：http://fqf.zhengqikj.top

split -l 1000 big.log part_
来源：http://fcm.jqgfzy.top

[R74] 批量重命名
来源：http://ihe.jianghu66.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://efg.zhongyouzk.top

[R75] 导出环境变量
来源：http://tdx.hesvh.cn

export PATH="$HOME/bin:$PATH"
来源：http://grt.ppjwa.cn

[R76] 使用临时文件
来源：http://fje.zhaomingkeji.xyz

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://erx.pycfn.com

[R77] 读取用户输入
来源：http://nef.dianchejie.cn

read -rp "请输入: " ans
来源：http://voi.svipenyu.cn

[R78] 交互式菜单
来源：http://veh.zhongyouzk.top

select opt in a b c; do echo "$opt"; break; done
来源：http://rkc.jyoumei.cn

[R79] 解析命令行选项
来源：http://gty.nanxuanxn.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://agn.guowangkeji.top

[R80] 查看脚本执行耗时
来源：http://agp.gotoacloud.top

time ./run.sh
来源：http://hqr.dianchejie.cn

================================================================================
来源：http://txs.andypj.xyz

S. C / C++ 专题
来源：http://pvb.bjfxy.top

================================================================================
来源：http://zvk.sjlbkw.cn

[S01] C：Hello World
来源：http://zzz.vqdsnc.cn

#include <stdio.h>
来源：http://rpz.ywan-chungtsiang.top

int main(void) { printf("Hello\n"); return 0; }
来源：http://zqv.cdnleiting.top

[S02] C：变量与格式化输出
来源：http://uyz.zhiwuduotai.top

int a = 10; printf("%d\n", a);
来源：http://vsm.shanyushiyangtech.top

[S03] C：读入整数
来源：http://mtr.dashuyun.cn

int x; scanf("%d", &x);
来源：http://nex.zhengqikj.top

[S04] C：字符串复制
来源：http://hqg.birdmap.top

char dst[32]; strcpy(dst, "hi");
来源：http://jpr.hesvh.cn

[S05] C：字符串长度
来源：http://nvp.shzxlz.cn

strlen(s)
来源：http://tzq.cashguo.top

[S06] C：字符串比较
来源：http://zhm.shangyingyoupin.top

strcmp(a, b) == 0
来源：http://umf.ydzc1.top

[S07] C：数组遍历求和
来源：http://who.zycfv.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xgt.ydjk.org.cn

[S08] C：动态内存分配与释放
来源：http://uaf.snrcjt.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wdr.kuanghao11.cn

[S09] C：结构体定义与初始化
来源：http://cea.xuetiantiany.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pix.daxiang520.top

[S10] C：指针与解引用
来源：http://nzs.yj20258888.top

int *p = &a;  *p = 5;
来源：http://tpm.snrcjt.cn

[S11] C：逐行读文件
来源：http://ucw.yueranfly.top

FILE *f = fopen("a.txt", "r");
来源：http://sdf.c1oappe.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://ezl.wangdashe.top

fclose(f);
来源：http://njh.zdqjudy.top

[S12] C：写文件
来源：http://gpg.hcnkem.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://scz.uphjek.com

[S13] C：宏定义
来源：http://qzm.epnwcf.com

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wdf.vehdjk.com

[S14] C：枚举
来源：http://ndm.shuidangran.top

enum Color { RED, GREEN, BLUE };
来源：http://fek.yanxiufei.cn

[S15] C：类型转换
来源：http://tmj.birdmap.top

(double) a / b
来源：http://zok.ywan-chungtsiang.top

[S16] C：位操作置位
来源：http://ejr.shangyingyoupin.top

x |= (1 << 3);
来源：http://bex.hongshengwenyu.top

[S17] C：安全拼接字符串
来源：http://scn.jlsjyb.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tfg.tianlin.xyz

[S18] C：命令行参数
来源：http://vzd.meibo888.top

int main(int argc, char **argv)
来源：http://dvo.meibo888.top

[S19] C：快速排序
来源：http://bpw.yueranfly.top

qsort(a, n, sizeof(int), cmp);
来源：http://aut.jinghuilouyu.cn

[S20] C：二分查找
来源：http://akb.fehbvm.com

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ald.c1oappe.top

[S21] C：字符类别判断
来源：http://hei.chenjidiqi.icu

isdigit(c);  isalpha(c);  isspace(c);
来源：http://tjr.ybcxt.top

[S22] C：字符串转数字
来源：http://zgf.c1oappe.top

atoi("42");  strtod("3.14", NULL);
来源：http://wsc.wangshuangyany.cn

[S23] C：随机数
来源：http://dwn.wangdashe.top

srand(time(NULL));  int r = rand() % 100;
来源：http://iap.yongpay.top

[S24] C：获取本地时间
来源：http://zda.xuetiantiany.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://usk.cucudq.cn

[S25] C：内存拷贝
来源：http://afa.dianchejie.cn

memcpy(dst, src, n);
来源：http://jly.vehdjk.com

[S26] C：内存清零
来源：http://rqg.ehwqpu.com

memset(a, 0, sizeof a);
来源：http://sfc.ybcxt.top

[S27] C：定义常量
来源：http://ati.ctjpmb.com

const double PI = 3.14159;
来源：http://swy.daxiang520.top

[S28] C：静态变量
来源：http://pkt.jinyuanbaomall.cn

static int counter = 0;
来源：http://qua.daxiang520.top

[S29] C：变参函数
来源：http://myx.cashguo.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hne.wangdashe.top

[S30] C：头文件保护
来源：http://rxj.9152youxi.cn

#ifndef X_H
来源：http://aye.yvedp.cn

#define X_H
来源：http://jiz.xylfe.cn

#endif
来源：http://xys.xingfuxueyuan.xyz

[S31] C++：Hello World
来源：http://qix.wangdashe.top

#include <iostream>
来源：http://rwh.cdnleiting.top

int main() { std::cout << "Hello\n"; }
来源：http://hrl.sufxvd.cn

[S32] C++：字符串
来源：http://fkk.tianlin.xyz

std::string s = "hi";  s += "!";
来源：http://pag.nanxuanxn.top

[S33] C++：vector 增删
来源：http://ppr.daxiang520.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cdv.fehbvm.com

[S34] C++：遍历 vector
来源：http://rlh.pycfn.com

for (auto &x : v) { std::cout << x; }
来源：http://wfs.havefunace.top

[S35] C++：map
来源：http://wei.yfazqb.com

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xhr.zycfv.cn

[S36] C++：unordered_map
来源：http://ymp.fktsv.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://azt.shanyushiyangtech.top

[S37] C++：set
来源：http://jyi.yonumen.top

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://huh.shzxlz.cn

[S38] C++：排序
来源：http://bna.bbcook.cn

std::sort(v.begin(), v.end());
来源：http://rnf.316326.xyz

[S39] C++：自定义比较器排序
来源：http://awq.ctjpmb.com

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bxe.dashuyun.cn

[S40] C++：查找元素
来源：http://yik.feifeiyinyue.top

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zcf.hfpthk.cn

[S41] C++：类与构造函数
来源：http://cbr.feifeiyinyue.top

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wwq.ywan-chungtsiang.top

[S42] C++：继承与虚函数
来源：http://ykv.jinyuanbaomall.cn

class B : public Base { public: void f() override {} };
来源：http://akl.gogol.net.cn

[S43] C++：智能指针
来源：http://jqm.cucudq.cn

auto p = std::make_unique<int>(5);
来源：http://gvv.yj202588.top

[S44] C++：引用传参
来源：http://xen.hywenlv.cn

void inc(int &x) { ++x; }
来源：http://civ.c1oappe.top

[S45] C++：lambda
来源：http://xuo.zdbjq.cn

auto add = [](int a, int b) { return a + b; };
来源：http://min.xinyue.icu

[S46] C++：函数模板
来源：http://ngd.zhixingplan.top

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://scf.ywan-chungtsiang.top

[S47] C++：结构化绑定遍历
来源：http://cxu.cashguo.top

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zlp.ydjk.org.cn

[S48] C++：逐行读文件
来源：http://yla.shangyingyoupin.top

std::ifstream in("a.txt");  std::string line;
来源：http://jwm.yj202588.top


<!-- 参考信息 -->