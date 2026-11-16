代发 wailian999

[Q65] 回滚事务
来源：http://thw.yj202588.top

ROLLBACK;
来源：http://igb.jyoumei.cn

[Q66] 行锁查询
来源：http://usg.yanxiufei.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://cck.shuidangran.top

[Q67] 设置隔离级别
来源：http://zow.quarkkingdee.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://rrj.uphjek.com

[Q68] 保存点
来源：http://oqa.yj20258888.top

SAVEPOINT sp1;
来源：http://tik.xingfuxueyuan.xyz

ROLLBACK TO sp1;
来源：http://izz.cheryme.top

[Q69] 查看执行计划
来源：http://cgg.tian-w.cn

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://qyr.bjfxy.top

[Q70] 更新统计信息
来源：http://qsb.gogol.net.cn

ANALYZE TABLE users;
来源：http://cpa.wangshuangyany.cn

[Q71] 查看建表语句
来源：http://dgu.yueranfly.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://hba.dianchejie.cn

[Q72] 查看索引
来源：http://lpw.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://hsn.yonumen.top

[Q73] 查看表状态
来源：http://kkw.zdbjq.cn

SHOW TABLE STATUS LIKE 'users';
来源：http://ppb.yj202588.top

[Q74] 强制使用索引
来源：http://vjn.zhongyouzk.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://sdv.jyoumei.cn

[Q75] 日期格式化
来源：http://opz.zhijiandao.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://vad.yj202588.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://uot.kuanghao11.cn

[Q76] 按天统计
来源：http://luc.c1oappe.top

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://vjv.chenjidiqi.icu

[Q77] 时间加减
来源：http://cfw.gzhubu.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://ohs.yuxming.cn

[Q78] 当前时间
来源：http://imo.aizwys.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://arg.nanxuanxn.top

[Q79] 字符串拼接
来源：http://chj.ydjk.org.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://qok.zhengqikj.top

[Q80] 字符串截取
来源：http://jyq.wangshuangyany.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mqz.sysykeji.top

[Q81] 字符串替换
来源：http://tiq.tanke756.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://rcm.ywan-chungtsiang.top

[Q82] 字符长度与字节长度
来源：http://yjl.nanxinkj.top

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://rhz.hongshengwenyu.top

[Q83] 大小写转换
来源：http://fgx.c1oappe.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://sgl.feifeiyinyue.top

[Q84] 去除首尾空格
来源：http://muf.sysykeji.top

SELECT TRIM(name) FROM users;
来源：http://nkk.fzhhl.top

[Q85] 数值取整
来源：http://wiv.guowangkeji.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://ctj.fengsongda.top

[Q86] 读取 JSON 字段
来源：http://fwn.pengpengdd.cyou

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://irl.fehbvm.com

[Q87] JSON 字段做条件
来源：http://yxr.9152youxi.cn

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://rog.zycfv.cn

[Q88] 行转列（条件聚合）
来源：http://iaa.shuidangran.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://utg.yangfankeji.com

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://hcg.shanyushiyangtech.top

[Q89] 判断表是否存在
来源：http://tto.chenzaomai.com

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fvp.cucudq.cn

[Q90] 生成序号列
来源：http://zgg.ehwqpu.com

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://ljv.jinghuilouyu.cn

================================================================================
来源：http://oag.fengsongda.top

R. Bash 专题
来源：http://jjr.iojbl.cn

================================================================================
来源：http://lts.zdqjudy.top

[R01] shebang 与严格模式
来源：http://fkk.tarul.cn

#!/usr/bin/env bash
来源：http://gki.shzxlz.cn

set -euo pipefail
来源：http://stz.haohaochexian.top

[R02] 变量赋值与使用
来源：http://ovd.pengpengdd.cyou

name="Tom"; echo "$name"
来源：http://lti.zhixingplan.top

[R03] 只读变量
来源：http://qnk.jinqigufen.top

readonly PI=3.14
来源：http://mjp.sweek.top

[R04] 位置参数
来源：http://ywx.yvedp.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://geb.ehwqpu.com

[R05] 参数默认值
来源：http://mtw.ivvv.top

name="${1:-default}"
来源：http://tar.cqqwz.cn

[R06] 判断命令是否存在
来源：http://jcd.vehdjk.com

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://ffv.yj202588.top

[R07] if 判断文件
来源：http://zvc.ctjpmb.com

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://kmv.dashuyun.cn

[R08] 数值比较
来源：http://fyh.yj202588.top

if (( a > b )); then echo "a 更大"; fi
来源：http://uki.hesvh.cn

[R09] 字符串比较
来源：http://snw.gaohongyu789.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://nui.vehdjk.com

[R10] 正则匹配
来源：http://yco.xingfuxueyuan.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://qaf.hongshengwenyu.top

[R11] case 多分支
来源：http://jgd.dashuyun.cn

case "$1" in
来源：http://agh.52xcode.cn

start) echo "启动" ;;
来源：http://anv.52xcode.cn

stop)  echo "停止" ;;
来源：http://xrr.xinyue.icu

*)     echo "未知命令" ;;
来源：http://lsa.guowangkeji.top

esac
来源：http://fne.yvedp.cn

[R12] for 遍历文件
来源：http://ufk.yvedp.cn

for f in *.txt; do echo "$f"; done
来源：http://wgj.jinyuanbaomall.cn

[R13] for 计数循环
来源：http://gmx.zhengqikj.top

for i in {1..10}; do echo "$i"; done
来源：http://vac.quarkkingdee.top

[R14] C 风格 for
来源：http://hkm.jqgufenzy.top

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://iwv.tarul.cn

[R15] while 逐行读文件
来源：http://git.hongshengwenyu.top

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://hnh.dashuyun.cn

[R16] until 等待条件
来源：http://wry.fanxiaobao.xyz

until [[ -f done.flag ]]; do sleep 1; done
来源：http://xfb.shanyushiyangtech.top

[R17] 数组定义与取值
来源：http://dcv.yj20258888.top

arr=(a b c); echo "${arr[0]}"
来源：http://kms.cdnleiting.top

[R18] 遍历数组
来源：http://geg.sxryk.cn

for x in "${arr[@]}"; do echo "$x"; done
来源：http://zfk.andypj.xyz

[R19] 数组长度
来源：http://ghz.dianchejie.cn

echo "${#arr[@]}"
来源：http://dee.52xcode.cn

[R20] 关联数组（字典）
来源：http://lrk.hysaishi.cn

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://stt.c1oappe.top

[R21] 字符串长度
来源：http://ltr.xinyue.icu

echo "${#s}"
来源：http://gjl.jlsjyb.cn

[R22] 截取子串
来源：http://caf.zhaomingkeji.xyz

echo "${s:0:5}"
来源：http://ldd.zhixingplan.top

[R23] 字符串替换
来源：http://mxq.wangshuangyany.cn

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://dfi.nanxuanxn.top

[R24] 大小写转换
来源：http://itr.wangdashe.top

echo "${s^^}"; echo "${s,,}"
来源：http://prt.uphjek.com

[R25] 去后缀 / 去前缀
来源：http://eiw.xingfuxueyuan.xyz

echo "${f%.txt}"; echo "${f#./}"
来源：http://mgf.316326.xyz

[R26] 命令替换
来源：http://lyq.dashuyun.cn

now=$(date +%F); echo "$now"
来源：http://koh.ehwqpu.com

[R27] 算术展开
来源：http://agy.sjlbkw.cn

echo $((1 + 2 * 3))
来源：http://hot.chenlongwang.top

[R28] 浮点运算
来源：http://wes.zhijiandao.cn

echo "scale=2; 10/3" | bc
来源：http://crg.zhengqikj.top

[R29] 定义函数
来源：http://pzw.yonumen.top

add() { echo $(($1 + $2)); }; add 1 2
来源：http://rkv.gotoacloud.top

[R30] 函数返回状态码
来源：http://nxc.xuanzx.com

f() { return 0; }; f || echo "失败了"
来源：http://zey.redwolf501.top

[R31] 局部变量
来源：http://vjb.xziqi.cn

f() { local x=1; echo "$x"; }
来源：http://sxb.wangshuangyany.cn

[R32] 参数个数校验
来源：http://aem.meibo888.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://alg.wangdashe.top

[R33] 捕获错误并提示行号
来源：http://gxq.52xcode.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://uta.chenlongwang.top

[R34] 退出时清理
来源：http://ngj.birdmap.top

trap 'rm -f "$tmp"' EXIT
来源：http://ymg.xuanzx.com

[R35] 后台执行并等待
来源：http://joh.yvedp.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://oil.guannengcc.top

[R36] 并发执行多个任务
来源：http://tre.tarul.cn

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://xnh.jinyuanbaomall.cn

[R37] 把输出赋给变量
来源：http://sbk.yuxming.cn

files=$(ls -1)
来源：http://qjf.cdnleiting.top

[R38] 管道串联
来源：http://xqs.svipenyu.cn

cat a.txt | grep -i error | wc -l
来源：http://mnz.kuanghao11.cn

[R39] 重定向标准输出与错误
来源：http://btf.hywenlv.cn

cmd > out.log 2>&1
来源：http://sgy.sufxvd.cn

[R40] 追加写日志
来源：http://ttt.hysaishi.cn

echo "log" >> out.log
来源：http://lsy.ydzc1.top

[R41] 丢弃输出
来源：http://yqd.andypj.xyz

cmd >/dev/null 2>&1
来源：http://okt.cdnleiting.top

[R42] 输入重定向
来源：http://ayy.shanyushiyangkeji.top

wc -l < a.txt
来源：http://gex.andypj.xyz

[R43] 按名字查找文件
来源：http://hbf.iojbl.cn

find . -name "*.log" -type f
来源：http://dyk.dianchejie.cn

[R44] 按修改时间查找
来源：http://rkq.ydjk.org.cn

find . -mtime -7 -type f
来源：http://uwb.ydzc1.top

[R45] 批量删除
来源：http://iec.0kj1m.cn

find . -name "*.tmp" -delete
来源：http://aus.ppjwa.cn

[R46] 递归替换文件内容
来源：http://rhi.nanxuanxn.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://jhx.fengsongda.top

[R47] sed 单行替换
来源：http://rxx.zhixingplan.top

sed -i 's/foo/bar/g' a.txt
来源：http://zgp.andypj.xyz

[R48] awk 取指定列
来源：http://rzq.9152youxi.cn

awk '{print $1, $3}' a.txt
来源：http://bnw.hysaishi.cn

[R49] awk 带条件
来源：http://otb.ivvv.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://aoh.ywan-chungtsiang.top

[R50] awk 求和
来源：http://hge.daxiang520.top

awk '{s += $2} END {print s}' a.txt
来源：http://ehn.meibo888.top

[R51] 排序去重取前几
来源：http://irq.tarul.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://qla.shanyushiyangkeji.top

[R52] 统计行数
来源：http://hgg.guannengcc.top

wc -l a.txt
来源：http://tkx.fzhhl.top

[R53] 查看文件头与实时尾
来源：http://vmt.tanke756.top

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://sbq.gogol.net.cn

[R54] 比较两个文件
来源：http://fyv.hongshengwenyu.top

diff a.txt b.txt
来源：http://ozt.zhengqikj.top

[R55] 压缩与解压
来源：http://chi.haohaochexian.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hnl.xuanzx.com

[R56] 远程拷贝
来源：http://vjp.nanxuanxn.top

scp file user@host:/path/
来源：http://jcd.cashguo.top

[R57] 远程执行命令
来源：http://pok.guowangkeji.top

ssh user@host 'uptime'
来源：http://yxw.xziqi.cn

[R58] 下载文件
来源：http://nzb.gzhubu.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://cqu.fzhhl.top

[R59] 发 POST JSON
来源：http://ebq.yj202588.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xsx.gzhubu.top

[R60] 只看 HTTP 状态码
来源：http://enl.zhongyouzk.top

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tub.yueranfly.top

[R61] 磁盘占用
来源：http://wkh.sufxvd.cn

df -h;  du -sh *
来源：http://ddj.jlsjyb.cn

[R62] 找最占空间的文件
来源：http://lod.daria6918.cn

du -ah . | sort -rh | head -10
来源：http://rts.wangdashe.top

[R63] 内存与进程
来源：http://nic.316326.xyz

free -h;  ps aux | grep nginx
来源：http://tqz.bbcook.cn

[R64] 结束进程
来源：http://nqg.nanxinkj.top

kill -9 $(pgrep -f app.py)
来源：http://dlu.zhijiandao.cn

[R65] 查看端口占用
来源：http://aqq.yongpay.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hhp.havefunace.top

[R66] 定时任务
来源：http://jpf.kuanghao11.cn

crontab -e;  crontab -l
来源：http://hge.ydzc1.top

[R67] 生成随机十六进制串
来源：http://jib.sjlbkw.cn

openssl rand -hex 16
来源：http://oaa.nanxinkj.top

[R68] 计算文件校验值
来源：http://lje.wangshuangyany.cn

sha256sum a.txt;  md5sum a.txt
来源：http://khr.yuxming.cn

[R69] 生成随机密码
来源：http://jtv.yangfankeji.com

head -c 16 /dev/urandom | base64
来源：http://uca.ydzc1.top

[R70] 时间戳与互转
来源：http://oqp.xingfuxueyuan.xyz

date +%s;  date -d @1700000000
来源：http://iaf.guowangkeji.top

[R71] 日期格式化
来源：http://wfi.jqgfzy.top

date +"%Y-%m-%d %H:%M:%S"
来源：http://qhi.yj20258888.top

[R72] 等待端口就绪
来源：http://vnk.yuxming.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ykq.cheryme.top

[R73] 分割大日志
来源：http://mho.jinghuilouyu.cn

split -l 1000 big.log part_
来源：http://imp.yonumen.top

[R74] 批量重命名
来源：http://lir.zhiwuduotai.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bql.fktsv.cn

[R75] 导出环境变量
来源：http://eec.mhx1999.top

export PATH="$HOME/bin:$PATH"
来源：http://xwa.chenjidiqi.icu

[R76] 使用临时文件
来源：http://viu.shuidangran.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hwv.xuetiantiany.cn

[R77] 读取用户输入
来源：http://oov.xuetiantiany.cn

read -rp "请输入: " ans
来源：http://gkw.andypj.xyz

[R78] 交互式菜单
来源：http://kfs.yongpay.top

select opt in a b c; do echo "$opt"; break; done
来源：http://xyc.tarul.cn

[R79] 解析命令行选项
来源：http://lhi.fengsongda.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pqh.dashuyun.cn

[R80] 查看脚本执行耗时
来源：http://qzx.nwbrower.top

time ./run.sh
来源：http://ety.zhixingplan.top

================================================================================
来源：http://tep.zhiwuduotai.top

S. C / C++ 专题
来源：http://qju.yj20258.top

================================================================================
来源：http://hzr.zhongyouzk.top

[S01] C：Hello World
来源：http://dxp.hnqzz.top

#include <stdio.h>
来源：http://sas.fehbvm.com

int main(void) { printf("Hello\n"); return 0; }
来源：http://tqe.sxryk.cn

[S02] C：变量与格式化输出
来源：http://nav.dianchejie.cn

int a = 10; printf("%d\n", a);
来源：http://ifm.9152youxi.cn

[S03] C：读入整数
来源：http://uon.xinyue.icu

int x; scanf("%d", &x);
来源：http://ddm.fzhhl.top

[S04] C：字符串复制
来源：http://mki.xingfuxueyuan.xyz

char dst[32]; strcpy(dst, "hi");
来源：http://vqd.jinghuilouyu.cn

[S05] C：字符串长度
来源：http://glh.9152youxi.cn

strlen(s)
来源：http://mzg.hnxiangtu.top

[S06] C：字符串比较
来源：http://snn.yongpay.top

strcmp(a, b) == 0
来源：http://juj.iojbl.cn

[S07] C：数组遍历求和
来源：http://qni.svipenyu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mjx.svipenyu.cn

[S08] C：动态内存分配与释放
来源：http://vch.guannengcc.top

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qpr.jqgufenzy.top

[S09] C：结构体定义与初始化
来源：http://ena.smart0.xyz

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dun.zhoulong.xyz

[S10] C：指针与解引用
来源：http://zhk.yuanzhike.top

int *p = &a;  *p = 5;
来源：http://svk.aibaodan.cn

[S11] C：逐行读文件
来源：http://tne.gotoacloud.top

FILE *f = fopen("a.txt", "r");
来源：http://wdv.yj20258.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://mcp.havefunace.top

fclose(f);
来源：http://zgu.xziqi.cn

[S12] C：写文件
来源：http://vru.chenzaomai.com

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nud.dashuyun.cn

[S13] C：宏定义
来源：http://ase.yanxiufei.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://btb.hysaishi.cn

[S14] C：枚举
来源：http://yut.yanxiufei.cn

enum Color { RED, GREEN, BLUE };
来源：http://ioz.zdbjq.cn

[S15] C：类型转换
来源：http://dmh.bjfxy.top

(double) a / b
来源：http://ajq.daria6918.cn

[S16] C：位操作置位
来源：http://pdf.chenjidiqi.icu

x |= (1 << 3);
来源：http://zsg.zhijiandao.cn

[S17] C：安全拼接字符串
来源：http://nlw.zhijiandao.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mxy.yfazqb.com

[S18] C：命令行参数
来源：http://rtb.hfpthk.cn

int main(int argc, char **argv)
来源：http://egp.shuidangran.top

[S19] C：快速排序
来源：http://klj.chenzaomai.com

qsort(a, n, sizeof(int), cmp);
来源：http://stx.daxiang520.top

[S20] C：二分查找
来源：http://nkn.sweek.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yxe.jqgfzy.top

[S21] C：字符类别判断
来源：http://ccr.jinghuilouyu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zuq.wangshuangyany.cn

[S22] C：字符串转数字
来源：http://clb.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vrx.havefunace.top

[S23] C：随机数
来源：http://crw.hnqzz.top

srand(time(NULL));  int r = rand() % 100;
来源：http://pij.hnqzz.top

[S24] C：获取本地时间
来源：http://btx.jianghu66.top

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zlx.hongshengwenyu.top

[S25] C：内存拷贝
来源：http://bpp.fanxiaobao.xyz

memcpy(dst, src, n);
来源：http://kpe.zhongyouzk.top

[S26] C：内存清零
来源：http://fum.zdbjq.cn

memset(a, 0, sizeof a);
来源：http://xil.gotoacloud.top

[S27] C：定义常量
来源：http://vxg.chenlongwang.top

const double PI = 3.14159;
来源：http://jjo.yongpay.top

[S28] C：静态变量
来源：http://dkj.chenzaomai.com

static int counter = 0;
来源：http://lsa.kuanghao11.cn

[S29] C：变参函数
来源：http://nbo.fktsv.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://dko.hongshengwenyu.top

[S30] C：头文件保护
来源：http://lna.svipenyu.cn

#ifndef X_H
来源：http://nay.cashguo.top

#define X_H
来源：http://hce.jianghu66.top

#endif
来源：http://cac.hnqzz.top

[S31] C++：Hello World
来源：http://fez.sweek.top

#include <iostream>
来源：http://znb.uphjek.com

int main() { std::cout << "Hello\n"; }
来源：http://pro.pycfn.com

[S32] C++：字符串
来源：http://xsb.cashguo.top

std::string s = "hi";  s += "!";
来源：http://bbr.gaohongyu789.top

[S33] C++：vector 增删
来源：http://edr.havefunace.top

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uwu.hongshengwenyu.top

[S34] C++：遍历 vector
来源：http://syw.jlsjyb.cn

for (auto &x : v) { std::cout << x; }
来源：http://ghq.zhongyouzk.top


<!-- 参考信息 -->