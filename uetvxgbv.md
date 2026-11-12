代发 wailian999

[Q61] 移动平均
来源：http://ukq.epnwcf.com

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://dte.yfazqb.com

[Q62] 分组占比
来源：http://nap.kuanghao11.cn

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://uen.feifeiyinyue.top

[Q63] 开启事务
来源：http://ylu.dashuyun.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://hwh.hnxiangtu.top

[Q64] 提交事务
来源：http://iex.chenlongwang.top

COMMIT;
来源：http://cbz.9152youxi.cn

[Q65] 回滚事务
来源：http://aee.ehwqpu.com

ROLLBACK;
来源：http://job.haohaochexian.top

[Q66] 行锁查询
来源：http://gmt.sysykeji.top

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://yzp.xingfuxueyuan.xyz

[Q67] 设置隔离级别
来源：http://our.yj20258.top

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://ufg.chenjidiqi.icu

[Q68] 保存点
来源：http://vsj.yuxming.cn

SAVEPOINT sp1;
来源：http://faf.hammf.cn

ROLLBACK TO sp1;
来源：http://ybp.nanxinkj.top

[Q69] 查看执行计划
来源：http://mwk.cheryme.top

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://knf.cashguo.top

[Q70] 更新统计信息
来源：http://qku.hysaishi.cn

ANALYZE TABLE users;
来源：http://mss.hfpthk.cn

[Q71] 查看建表语句
来源：http://keh.zhiwuduotai.top

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://qup.aizwys.cn

[Q72] 查看索引
来源：http://uym.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://jqy.jinqigufen.top

[Q73] 查看表状态
来源：http://joc.feifeiyinyue.top

SHOW TABLE STATUS LIKE 'users';
来源：http://rol.guowangkeji.top

[Q74] 强制使用索引
来源：http://iwi.nanxuanxn.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://poa.52xcode.cn

[Q75] 日期格式化
来源：http://xmk.yuxming.cn

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://myb.jqgufenzy.top

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ltl.guannengcc.top

[Q76] 按天统计
来源：http://hzz.daria6918.cn

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://csr.havefunace.top

[Q77] 时间加减
来源：http://dkw.0kj1m.cn

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://nxb.cheryme.top

[Q78] 当前时间
来源：http://jah.bbcook.cn

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://hmk.yangfankeji.com

[Q79] 字符串拼接
来源：http://fxt.pengpengdd.cyou

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://tfg.9152youxi.cn

[Q80] 字符串截取
来源：http://ipf.jlsjyb.cn

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mbw.gotoacloud.top

[Q81] 字符串替换
来源：http://pty.jyoumei.cn

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://fzd.bbcook.cn

[Q82] 字符长度与字节长度
来源：http://cut.svipenyu.cn

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://sdm.yanxiufei.cn

[Q83] 大小写转换
来源：http://mod.jqgufenzy.top

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://kqm.iojbl.cn

[Q84] 去除首尾空格
来源：http://zyf.feifeiyinyue.top

SELECT TRIM(name) FROM users;
来源：http://wlg.gaohongyu789.top

[Q85] 数值取整
来源：http://ime.yongpay.top

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://yqz.fehbvm.com

[Q86] 读取 JSON 字段
来源：http://lcd.snrcjt.cn

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://let.52xcode.cn

[Q87] JSON 字段做条件
来源：http://daa.wangdashe.top

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kvw.fanxiaobao.xyz

[Q88] 行转列（条件聚合）
来源：http://zvd.zhiwuduotai.top

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://zds.aibaodan.cn

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://igr.0kj1m.cn

[Q89] 判断表是否存在
来源：http://fvi.gzhubu.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://vpw.iojbl.cn

[Q90] 生成序号列
来源：http://gpb.aizwys.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://xmt.zhiwuduotai.top

================================================================================
来源：http://bhr.xziqi.cn

R. Bash 专题
来源：http://xzu.jianghu66.top

================================================================================
来源：http://qcx.nanxuanxn.top

[R01] shebang 与严格模式
来源：http://pfo.chenlongwang.top

#!/usr/bin/env bash
来源：http://byi.jianghu66.top

set -euo pipefail
来源：http://gmq.birdmap.top

[R02] 变量赋值与使用
来源：http://oam.yonumen.top

name="Tom"; echo "$name"
来源：http://ext.birdmap.top

[R03] 只读变量
来源：http://dtc.pycfn.com

readonly PI=3.14
来源：http://kzf.hfpthk.cn

[R04] 位置参数
来源：http://amn.fzhhl.top

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://for.jqgfzy.top

[R05] 参数默认值
来源：http://nuo.hnqzz.top

name="${1:-default}"
来源：http://xao.shzxlz.cn

[R06] 判断命令是否存在
来源：http://iiz.yuxming.cn

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://kwd.yuanzhike.top

[R07] if 判断文件
来源：http://afr.fktsv.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://hit.hammf.cn

[R08] 数值比较
来源：http://fwm.jqgufenzy.top

if (( a > b )); then echo "a 更大"; fi
来源：http://cve.havefunace.top

[R09] 字符串比较
来源：http://xeh.yj20258888.top

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wqv.xuanzx.com

[R10] 正则匹配
来源：http://cws.tianlin.xyz

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://rml.daria6918.cn

[R11] case 多分支
来源：http://dwl.daxiang520.top

case "$1" in
来源：http://wdn.mhx1999.top

start) echo "启动" ;;
来源：http://hrj.haohaochexian.top

stop)  echo "停止" ;;
来源：http://iei.cheryme.top

*)     echo "未知命令" ;;
来源：http://iai.yueranfly.top

esac
来源：http://byp.shuidangran.top

[R12] for 遍历文件
来源：http://tsb.jinqigufen.top

for f in *.txt; do echo "$f"; done
来源：http://qiu.yuxming.cn

[R13] for 计数循环
来源：http://pod.ppjwa.cn

for i in {1..10}; do echo "$i"; done
来源：http://wiz.zhoulong.xyz

[R14] C 风格 for
来源：http://vjr.316326.xyz

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://gjw.dianchejie.cn

[R15] while 逐行读文件
来源：http://poy.yangfankeji.com

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://xzl.xylfe.cn

[R16] until 等待条件
来源：http://qok.yvedp.cn

until [[ -f done.flag ]]; do sleep 1; done
来源：http://qwj.sweek.top

[R17] 数组定义与取值
来源：http://ipy.gaohongyu789.top

arr=(a b c); echo "${arr[0]}"
来源：http://znt.hesvh.cn

[R18] 遍历数组
来源：http://uki.zhaomingkeji.xyz

for x in "${arr[@]}"; do echo "$x"; done
来源：http://oiv.feifeiyinyue.top

[R19] 数组长度
来源：http://xmn.yj202588.top

echo "${#arr[@]}"
来源：http://iqa.daxiang520.top

[R20] 关联数组（字典）
来源：http://rgz.ctjpmb.com

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://xij.zhengqikj.top

[R21] 字符串长度
来源：http://baz.sufxvd.cn

echo "${#s}"
来源：http://lgy.yueranfly.top

[R22] 截取子串
来源：http://wfw.ctjpmb.com

echo "${s:0:5}"
来源：http://pnz.dianchejie.cn

[R23] 字符串替换
来源：http://aso.feifeiyinyue.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://ljr.uphjek.com

[R24] 大小写转换
来源：http://svo.kuanghao11.cn

echo "${s^^}"; echo "${s,,}"
来源：http://poa.yj20258.top

[R25] 去后缀 / 去前缀
来源：http://yrr.bbcook.cn

echo "${f%.txt}"; echo "${f#./}"
来源：http://yxi.sufxvd.cn

[R26] 命令替换
来源：http://iux.shanyushiyangkeji.top

now=$(date +%F); echo "$now"
来源：http://qmm.ctjpmb.com

[R27] 算术展开
来源：http://wph.jyoumei.cn

echo $((1 + 2 * 3))
来源：http://myi.tarul.cn

[R28] 浮点运算
来源：http://aal.xylfe.cn

echo "scale=2; 10/3" | bc
来源：http://ngm.sysykeji.top

[R29] 定义函数
来源：http://wtu.xingfuxueyuan.xyz

add() { echo $(($1 + $2)); }; add 1 2
来源：http://gdm.cashguo.top

[R30] 函数返回状态码
来源：http://dgf.cashguo.top

f() { return 0; }; f || echo "失败了"
来源：http://auz.0kj1m.cn

[R31] 局部变量
来源：http://lxx.hywenlv.cn

f() { local x=1; echo "$x"; }
来源：http://odt.zhixingplan.top

[R32] 参数个数校验
来源：http://bnl.yongpay.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://imq.yanxiufei.cn

[R33] 捕获错误并提示行号
来源：http://bzo.dashuyun.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://vfc.daxiang520.top

[R34] 退出时清理
来源：http://ffw.tarul.cn

trap 'rm -f "$tmp"' EXIT
来源：http://gdp.zhoulong.xyz

[R35] 后台执行并等待
来源：http://wgx.shanyushiyangtech.top

sleep 5 & pid=$!; wait "$pid"
来源：http://ewm.tianlin.xyz

[R36] 并发执行多个任务
来源：http://ylp.bjfxy.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://pjp.316326.xyz

[R37] 把输出赋给变量
来源：http://vts.xuetiantiany.cn

files=$(ls -1)
来源：http://qkl.wangshuangyany.cn

[R38] 管道串联
来源：http://ybm.vehdjk.com

cat a.txt | grep -i error | wc -l
来源：http://ghz.c1oappe.top

[R39] 重定向标准输出与错误
来源：http://hrv.yonumen.top

cmd > out.log 2>&1
来源：http://cak.gotoacloud.top

[R40] 追加写日志
来源：http://znk.fanxiaobao.xyz

echo "log" >> out.log
来源：http://ubu.fktsv.cn

[R41] 丢弃输出
来源：http://twp.guowangkeji.top

cmd >/dev/null 2>&1
来源：http://ldi.jianghu66.top

[R42] 输入重定向
来源：http://jag.shanyushiyangtech.top

wc -l < a.txt
来源：http://qmn.jinyuanbaomall.cn

[R43] 按名字查找文件
来源：http://fdp.sufxvd.cn

find . -name "*.log" -type f
来源：http://vvi.svipenyu.cn

[R44] 按修改时间查找
来源：http://yhs.tian-w.cn

find . -mtime -7 -type f
来源：http://lxd.yfazqb.com

[R45] 批量删除
来源：http://cdy.guowangkeji.top

find . -name "*.tmp" -delete
来源：http://tpk.cqqwz.cn

[R46] 递归替换文件内容
来源：http://agu.cashguo.top

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://bvq.bbcook.cn

[R47] sed 单行替换
来源：http://wqo.316326.xyz

sed -i 's/foo/bar/g' a.txt
来源：http://xgw.jqgfzy.top

[R48] awk 取指定列
来源：http://zfj.pengpengdd.cyou

awk '{print $1, $3}' a.txt
来源：http://req.cashguo.top

[R49] awk 带条件
来源：http://tlc.yueranfly.top

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://yqm.ehwqpu.com

[R50] awk 求和
来源：http://foy.fengsongda.top

awk '{s += $2} END {print s}' a.txt
来源：http://lym.xinyue.icu

[R51] 排序去重取前几
来源：http://nno.smart0.xyz

sort a.txt | uniq -c | sort -rn | head
来源：http://siu.birdmap.top

[R52] 统计行数
来源：http://yhx.fengsongda.top

wc -l a.txt
来源：http://upg.9152youxi.cn

[R53] 查看文件头与实时尾
来源：http://paj.snrcjt.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://dge.hywenlv.cn

[R54] 比较两个文件
来源：http://jjr.sjlbkw.cn

diff a.txt b.txt
来源：http://mle.zhaomingkeji.xyz

[R55] 压缩与解压
来源：http://nbe.gogol.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xtq.yanxiufei.cn

[R56] 远程拷贝
来源：http://yhx.hysaishi.cn

scp file user@host:/path/
来源：http://bth.fanxiaobao.xyz

[R57] 远程执行命令
来源：http://loe.fengsongda.top

ssh user@host 'uptime'
来源：http://dhn.chenzaomai.com

[R58] 下载文件
来源：http://hlz.redwolf501.top

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://hnq.sweek.top

[R59] 发 POST JSON
来源：http://tej.ybcxt.top

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://tkk.gogol.net.cn

[R60] 只看 HTTP 状态码
来源：http://rgz.zhaomingkeji.xyz

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://giv.yongpay.top

[R61] 磁盘占用
来源：http://orp.fehbvm.com

df -h;  du -sh *
来源：http://tiq.havefunace.top

[R62] 找最占空间的文件
来源：http://kxr.xuanzx.com

du -ah . | sort -rh | head -10
来源：http://kzp.ppjwa.cn

[R63] 内存与进程
来源：http://soq.pengpengdd.cyou

free -h;  ps aux | grep nginx
来源：http://xjp.dianchejie.cn

[R64] 结束进程
来源：http://qbx.fengsongda.top

kill -9 $(pgrep -f app.py)
来源：http://kjl.nanxuanxn.top

[R65] 查看端口占用
来源：http://qzl.quarkkingdee.top

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://oyo.smart0.xyz

[R66] 定时任务
来源：http://uoi.hywenlv.cn

crontab -e;  crontab -l
来源：http://skc.hnxiangtu.top

[R67] 生成随机十六进制串
来源：http://lgf.jiagoushi.top

openssl rand -hex 16
来源：http://fub.hnxiangtu.top

[R68] 计算文件校验值
来源：http://lwf.0kj1m.cn

sha256sum a.txt;  md5sum a.txt
来源：http://slz.yfazqb.com

[R69] 生成随机密码
来源：http://tvx.haohaochexian.top

head -c 16 /dev/urandom | base64
来源：http://fzw.52xcode.cn

[R70] 时间戳与互转
来源：http://myr.yj202588.top

date +%s;  date -d @1700000000
来源：http://bne.jyoumei.cn

[R71] 日期格式化
来源：http://rwu.ehwqpu.com

date +"%Y-%m-%d %H:%M:%S"
来源：http://tkr.feifeiyinyue.top

[R72] 等待端口就绪
来源：http://ppb.ywan-chungtsiang.top

until nc -z localhost 3306; do sleep 1; done
来源：http://jls.hesvh.cn

[R73] 分割大日志
来源：http://joh.jqgfzy.top

split -l 1000 big.log part_
来源：http://tyn.hfpthk.cn

[R74] 批量重命名
来源：http://cgd.jinqigfzy.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pnz.smart0.xyz

[R75] 导出环境变量
来源：http://nxh.zdqjudy.top

export PATH="$HOME/bin:$PATH"
来源：http://ead.hnxiangtu.top

[R76] 使用临时文件
来源：http://adr.xinyue.icu

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bjg.hesvh.cn

[R77] 读取用户输入
来源：http://iov.hysaishi.cn

read -rp "请输入: " ans
来源：http://hpu.ywan-chungtsiang.top

[R78] 交互式菜单
来源：http://nef.fktsv.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oyg.fzhhl.top

[R79] 解析命令行选项
来源：http://fgk.52xcode.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://isx.xinyue.icu

[R80] 查看脚本执行耗时
来源：http://uog.fzhhl.top

time ./run.sh
来源：http://htv.zdqjudy.top

================================================================================
来源：http://xow.zdqjudy.top

S. C / C++ 专题
来源：http://mcd.yueranfly.top

================================================================================
来源：http://nhj.bjfxy.top

[S01] C：Hello World
来源：http://zxi.redwolf501.top

#include <stdio.h>
来源：http://qef.zhijiandao.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://tqk.cashguo.top

[S02] C：变量与格式化输出
来源：http://puw.jyoumei.cn

int a = 10; printf("%d\n", a);
来源：http://ltm.zhiwuduotai.top

[S03] C：读入整数
来源：http://hbd.yangfankeji.com

int x; scanf("%d", &x);
来源：http://dcl.jianghu66.top

[S04] C：字符串复制
来源：http://tao.yanxiufei.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xho.shanyushiyangtech.top

[S05] C：字符串长度
来源：http://bwz.jinqigufen.top

strlen(s)
来源：http://csz.cqqwz.cn

[S06] C：字符串比较
来源：http://tex.cheryme.top

strcmp(a, b) == 0
来源：http://cuc.xylfe.cn

[S07] C：数组遍历求和
来源：http://vjf.dianchejie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ofa.yanxiufei.cn

[S08] C：动态内存分配与释放
来源：http://zlh.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zwc.shangyingyoupin.top

[S09] C：结构体定义与初始化
来源：http://lai.shanyushiyangtech.top

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mae.smart0.xyz

[S10] C：指针与解引用
来源：http://pty.fktsv.cn

int *p = &a;  *p = 5;
来源：http://csz.fzhhl.top

[S11] C：逐行读文件
来源：http://yyq.hcnkem.com

FILE *f = fopen("a.txt", "r");
来源：http://mkt.dashuyun.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://est.xuanzx.com

fclose(f);
来源：http://eed.hammf.cn

[S12] C：写文件
来源：http://klz.ydzc1.top

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xey.mhx1999.top

[S13] C：宏定义
来源：http://zqa.sysykeji.top

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://epu.guowangkeji.top

[S14] C：枚举
来源：http://sqp.guannengcc.top

enum Color { RED, GREEN, BLUE };
来源：http://cmw.daria6918.cn

[S15] C：类型转换
来源：http://wxr.wangdashe.top

(double) a / b
来源：http://cjs.yvedp.cn

[S16] C：位操作置位
来源：http://ewf.pycfn.com

x |= (1 << 3);
来源：http://ezm.c1oappe.top

[S17] C：安全拼接字符串
来源：http://dct.jinqigufen.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mvx.pengpengdd.cyou

[S18] C：命令行参数
来源：http://hvb.aibaodan.cn

int main(int argc, char **argv)
来源：http://vqa.ehwqpu.com

[S19] C：快速排序
来源：http://bag.smart0.xyz

qsort(a, n, sizeof(int), cmp);
来源：http://bgz.zhoulong.xyz

[S20] C：二分查找
来源：http://dnk.yueranfly.top

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tlm.hysaishi.cn

[S21] C：字符类别判断
来源：http://arf.shanyushiyangtech.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ixp.hongshengwenyu.top

[S22] C：字符串转数字
来源：http://ixk.fktsv.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uwo.sjlbkw.cn

[S23] C：随机数
来源：http://omk.tianlin.xyz

srand(time(NULL));  int r = rand() % 100;
来源：http://nft.nanxinkj.top

[S24] C：获取本地时间
来源：http://avr.xziqi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://esg.jlsjyb.cn

[S25] C：内存拷贝
来源：http://qrx.cashguo.top

memcpy(dst, src, n);
来源：http://mtn.gzhubu.top

[S26] C：内存清零
来源：http://axi.hammf.cn

memset(a, 0, sizeof a);
来源：http://eft.yj20258888.top

[S27] C：定义常量
来源：http://abf.ybcxt.top

const double PI = 3.14159;
来源：http://aat.ybcxt.top

[S28] C：静态变量
来源：http://fua.sysykeji.top

static int counter = 0;
来源：http://tcp.fengsongda.top

[S29] C：变参函数
来源：http://nxe.yj20258888.top

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://omj.jiagoushi.top

[S30] C：头文件保护
来源：http://unh.jinghuilouyu.cn

#ifndef X_H
来源：http://hdm.gzhubu.top

#define X_H
来源：http://fjc.ydzc1.top

#endif
来源：http://fdk.jqgufenzy.top

[S31] C++：Hello World
来源：http://dcv.xziqi.cn


<!-- 参考信息 -->