代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://tuf.jinqigfzy.top

[Q58] 累计求和
来源：http://maj.zhongyouzk.top

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mmr.yangfankeji.com

[Q59] 分组内累计
来源：http://prx.shzxlz.cn

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://ewo.chenlongwang.top

[Q60] 取上一行 / 下一行
来源：http://wtu.zhixingplan.top

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://hsb.shangyingyoupin.top

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://iun.jyoumei.cn

[Q61] 移动平均
来源：http://vgo.52xcode.cn

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://lxf.hesvh.cn

[Q62] 分组占比
来源：http://dtx.pengpengdd.cyou

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://ipk.redwolf501.top

[Q63] 开启事务
来源：http://cul.dianchejie.cn

START TRANSACTION;                -- 或 BEGIN
来源：http://vpg.hongshengwenyu.top

[Q64] 提交事务
来源：http://zii.ywan-chungtsiang.top

COMMIT;
来源：http://vlj.vqdsnc.cn

[Q65] 回滚事务
来源：http://qch.tanke756.top

ROLLBACK;
来源：http://rrf.jyoumei.cn

[Q66] 行锁查询
来源：http://ywb.gogol.net.cn

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://ujn.feifeiyinyue.top

[Q67] 设置隔离级别
来源：http://qyc.dashuyun.cn

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://hoq.zhoulong.xyz

[Q68] 保存点
来源：http://ulz.epnwcf.com

SAVEPOINT sp1;
来源：http://kib.jinyuanbaomall.cn

ROLLBACK TO sp1;
来源：http://thr.kuanghao11.cn

[Q69] 查看执行计划
来源：http://str.yangfankeji.com

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://pbi.yuxming.cn

[Q70] 更新统计信息
来源：http://lsi.shuidangran.top

ANALYZE TABLE users;
来源：http://tla.xylfe.cn

[Q71] 查看建表语句
来源：http://fem.bbcook.cn

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://thh.xingfuxueyuan.xyz

[Q72] 查看索引
来源：http://pds.shangyingyoupin.top

SHOW INDEX FROM users;
来源：http://nym.hnxiangtu.top

[Q73] 查看表状态
来源：http://cvb.smart0.xyz

SHOW TABLE STATUS LIKE 'users';
来源：http://agk.hnqzz.top

[Q74] 强制使用索引
来源：http://qfv.quarkkingdee.top

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://knj.sysykeji.top

[Q75] 日期格式化
来源：http://qvb.yongpay.top

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://nlt.sjlbkw.cn

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://ctk.hammf.cn

[Q76] 按天统计
来源：http://rft.fanxiaobao.xyz

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://whk.zycfv.cn

[Q77] 时间加减
来源：http://raq.feifeiyinyue.top

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://eaw.cqqwz.cn

[Q78] 当前时间
来源：http://yqn.uphjek.com

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://iyk.jqgfzy.top

[Q79] 字符串拼接
来源：http://xuq.ppjwa.cn

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://oeb.pycfn.com

[Q80] 字符串截取
来源：http://qnv.pengpengdd.cyou

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://igk.nanxinkj.top

[Q81] 字符串替换
来源：http://xvn.birdmap.top

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://kev.cqqwz.cn

[Q82] 字符长度与字节长度
来源：http://rtj.vehdjk.com

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://xon.zhijiandao.cn

[Q83] 大小写转换
来源：http://uke.gogol.net.cn

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://dvy.cqqwz.cn

[Q84] 去除首尾空格
来源：http://nxz.daria6918.cn

SELECT TRIM(name) FROM users;
来源：http://eyj.jinqigufen.top

[Q85] 数值取整
来源：http://yjl.xziqi.cn

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://klq.cashguo.top

[Q86] 读取 JSON 字段
来源：http://nsh.smart0.xyz

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://oin.yonumen.top

[Q87] JSON 字段做条件
来源：http://kgh.hcnkem.com

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://kff.tarul.cn

[Q88] 行转列（条件聚合）
来源：http://mam.cqqwz.cn

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://vkb.tianlin.xyz

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://dsb.cucudq.cn

[Q89] 判断表是否存在
来源：http://ehm.shanyushiyangtech.top

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://fny.vehdjk.com

[Q90] 生成序号列
来源：http://rqo.fktsv.cn

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://nao.yuxming.cn

================================================================================
来源：http://for.yongpay.top

R. Bash 专题
来源：http://viw.havefunace.top

================================================================================
来源：http://cas.wangshuangyany.cn

[R01] shebang 与严格模式
来源：http://qzg.wangshuangyany.cn

#!/usr/bin/env bash
来源：http://ukw.havefunace.top

set -euo pipefail
来源：http://voc.zdqjudy.top

[R02] 变量赋值与使用
来源：http://xet.vqdsnc.cn

name="Tom"; echo "$name"
来源：http://cgq.hesvh.cn

[R03] 只读变量
来源：http://dwu.sxryk.cn

readonly PI=3.14
来源：http://rlm.hammf.cn

[R04] 位置参数
来源：http://rmr.bbcook.cn

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://yee.xuetiantiany.cn

[R05] 参数默认值
来源：http://ecq.jqgfzy.top

name="${1:-default}"
来源：http://lqx.bbcook.cn

[R06] 判断命令是否存在
来源：http://fvi.shanyushiyangkeji.top

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://cga.chenzaomai.com

[R07] if 判断文件
来源：http://rrk.cucudq.cn

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://xts.daxiang520.top

[R08] 数值比较
来源：http://afn.gzhubu.top

if (( a > b )); then echo "a 更大"; fi
来源：http://ezw.316326.xyz

[R09] 字符串比较
来源：http://dnu.yanxiufei.cn

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wxq.yuxming.cn

[R10] 正则匹配
来源：http://rqq.ywan-chungtsiang.top

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://ffz.xziqi.cn

[R11] case 多分支
来源：http://wws.hnxiangtu.top

case "$1" in
来源：http://ccv.ydzc1.top

start) echo "启动" ;;
来源：http://bjb.tianlin.xyz

stop)  echo "停止" ;;
来源：http://ggn.daria6918.cn

*)     echo "未知命令" ;;
来源：http://ogc.sufxvd.cn

esac
来源：http://ilm.zhengqikj.top

[R12] for 遍历文件
来源：http://mcb.xuanzx.com

for f in *.txt; do echo "$f"; done
来源：http://mkm.jiagoushi.top

[R13] for 计数循环
来源：http://csr.yuxming.cn

for i in {1..10}; do echo "$i"; done
来源：http://lwm.ehwqpu.com

[R14] C 风格 for
来源：http://msq.yangfankeji.com

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://svz.gzhubu.top

[R15] while 逐行读文件
来源：http://spj.zdbjq.cn

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://shn.yanxiufei.cn

[R16] until 等待条件
来源：http://mny.ybcxt.top

until [[ -f done.flag ]]; do sleep 1; done
来源：http://lip.nanxinkj.top

[R17] 数组定义与取值
来源：http://kul.zhengqikj.top

arr=(a b c); echo "${arr[0]}"
来源：http://eqa.xinyue.icu

[R18] 遍历数组
来源：http://ybd.shuidangran.top

for x in "${arr[@]}"; do echo "$x"; done
来源：http://awe.gaohongyu789.top

[R19] 数组长度
来源：http://nib.yueranfly.top

echo "${#arr[@]}"
来源：http://zvg.yj20258.top

[R20] 关联数组（字典）
来源：http://tra.zhoulong.xyz

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://qwe.jinyuanbaomall.cn

[R21] 字符串长度
来源：http://noc.sxryk.cn

echo "${#s}"
来源：http://jpo.ybcxt.top

[R22] 截取子串
来源：http://mwv.yuanzhike.top

echo "${s:0:5}"
来源：http://yuf.gogol.net.cn

[R23] 字符串替换
来源：http://qro.yj20258.top

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://fyv.chenjidiqi.icu

[R24] 大小写转换
来源：http://jus.uphjek.com

echo "${s^^}"; echo "${s,,}"
来源：http://utg.xziqi.cn

[R25] 去后缀 / 去前缀
来源：http://zmk.zhiwuduotai.top

echo "${f%.txt}"; echo "${f#./}"
来源：http://rbo.epnwcf.com

[R26] 命令替换
来源：http://srj.jinqigufen.top

now=$(date +%F); echo "$now"
来源：http://vmh.zhiwuduotai.top

[R27] 算术展开
来源：http://qzk.zdqjudy.top

echo $((1 + 2 * 3))
来源：http://alw.sweek.top

[R28] 浮点运算
来源：http://vbp.vqdsnc.cn

echo "scale=2; 10/3" | bc
来源：http://dea.shuidangran.top

[R29] 定义函数
来源：http://fyv.52xcode.cn

add() { echo $(($1 + $2)); }; add 1 2
来源：http://xui.yj20258888.top

[R30] 函数返回状态码
来源：http://jgl.jqgfzy.top

f() { return 0; }; f || echo "失败了"
来源：http://ljb.hywenlv.cn

[R31] 局部变量
来源：http://obn.aibaodan.cn

f() { local x=1; echo "$x"; }
来源：http://xjc.shanyushiyangtech.top

[R32] 参数个数校验
来源：http://rwp.yonumen.top

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://xal.cashguo.top

[R33] 捕获错误并提示行号
来源：http://syp.zdbjq.cn

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://dgs.gotoacloud.top

[R34] 退出时清理
来源：http://yuw.uphjek.com

trap 'rm -f "$tmp"' EXIT
来源：http://ltq.cheryme.top

[R35] 后台执行并等待
来源：http://dto.aibaodan.cn

sleep 5 & pid=$!; wait "$pid"
来源：http://goj.yanxiufei.cn

[R36] 并发执行多个任务
来源：http://bwc.c1oappe.top

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://khg.c1oappe.top

[R37] 把输出赋给变量
来源：http://yyo.shzxlz.cn

files=$(ls -1)
来源：http://rmq.feifeiyinyue.top

[R38] 管道串联
来源：http://izl.cdnleiting.top

cat a.txt | grep -i error | wc -l
来源：http://vlp.aizwys.cn

[R39] 重定向标准输出与错误
来源：http://oxk.pengpengdd.cyou

cmd > out.log 2>&1
来源：http://acv.jinqigfzy.top

[R40] 追加写日志
来源：http://exm.c1oappe.top

echo "log" >> out.log
来源：http://zki.shzxlz.cn

[R41] 丢弃输出
来源：http://bas.hnqzz.top

cmd >/dev/null 2>&1
来源：http://jpa.guannengcc.top

[R42] 输入重定向
来源：http://wer.xylfe.cn

wc -l < a.txt
来源：http://ebr.jinqigfzy.top

[R43] 按名字查找文件
来源：http://cvg.xylfe.cn

find . -name "*.log" -type f
来源：http://wyp.aizwys.cn

[R44] 按修改时间查找
来源：http://hmc.yanxiufei.cn

find . -mtime -7 -type f
来源：http://syi.hongshengwenyu.top

[R45] 批量删除
来源：http://nij.yuanzhike.top

find . -name "*.tmp" -delete
来源：http://cig.aizwys.cn

[R46] 递归替换文件内容
来源：http://xbc.jinghuilouyu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://xpy.hongshengwenyu.top

[R47] sed 单行替换
来源：http://rjs.yvedp.cn

sed -i 's/foo/bar/g' a.txt
来源：http://ckc.xuetiantiany.cn

[R48] awk 取指定列
来源：http://xrc.cashguo.top

awk '{print $1, $3}' a.txt
来源：http://veo.xuanzx.com

[R49] awk 带条件
来源：http://qbd.hesvh.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wyx.quarkkingdee.top

[R50] awk 求和
来源：http://zzm.feifeiyinyue.top

awk '{s += $2} END {print s}' a.txt
来源：http://nmz.yanxiufei.cn

[R51] 排序去重取前几
来源：http://hyv.zycfv.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://lqv.pengpengdd.cyou

[R52] 统计行数
来源：http://vjm.chenzaomai.com

wc -l a.txt
来源：http://wok.hongshengwenyu.top

[R53] 查看文件头与实时尾
来源：http://dcx.fktsv.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rdh.andypj.xyz

[R54] 比较两个文件
来源：http://yqv.xinyue.icu

diff a.txt b.txt
来源：http://uza.hammf.cn

[R55] 压缩与解压
来源：http://lji.ybcxt.top

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ccn.daria6918.cn

[R56] 远程拷贝
来源：http://hrc.iojbl.cn

scp file user@host:/path/
来源：http://ksr.guowangkeji.top

[R57] 远程执行命令
来源：http://cxd.316326.xyz

ssh user@host 'uptime'
来源：http://cmt.tanke756.top

[R58] 下载文件
来源：http://tpf.tian-w.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ekm.jyoumei.cn

[R59] 发 POST JSON
来源：http://fwz.aizwys.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wzd.dianchejie.cn

[R60] 只看 HTTP 状态码
来源：http://icj.gogol.net.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ldz.quarkkingdee.top

[R61] 磁盘占用
来源：http://wrk.fehbvm.com

df -h;  du -sh *
来源：http://wwp.316326.xyz

[R62] 找最占空间的文件
来源：http://cjn.mhx1999.top

du -ah . | sort -rh | head -10
来源：http://olu.52xcode.cn

[R63] 内存与进程
来源：http://ajb.0kj1m.cn

free -h;  ps aux | grep nginx
来源：http://add.shangyingyoupin.top

[R64] 结束进程
来源：http://qkj.cucudq.cn

kill -9 $(pgrep -f app.py)
来源：http://uer.haohaochexian.top

[R65] 查看端口占用
来源：http://vth.dianchejie.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mzi.tanke756.top

[R66] 定时任务
来源：http://xbk.hcnkem.com

crontab -e;  crontab -l
来源：http://pfb.yangfankeji.com

[R67] 生成随机十六进制串
来源：http://hvu.yj20258.top

openssl rand -hex 16
来源：http://kap.aizwys.cn

[R68] 计算文件校验值
来源：http://tsg.vehdjk.com

sha256sum a.txt;  md5sum a.txt
来源：http://fkt.bbcook.cn

[R69] 生成随机密码
来源：http://ult.xinyue.icu

head -c 16 /dev/urandom | base64
来源：http://gyb.jinyuanbaomall.cn

[R70] 时间戳与互转
来源：http://nnt.sufxvd.cn

date +%s;  date -d @1700000000
来源：http://ydj.hnqzz.top

[R71] 日期格式化
来源：http://clf.sjlbkw.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dtc.havefunace.top

[R72] 等待端口就绪
来源：http://tqg.9152youxi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vih.yvedp.cn

[R73] 分割大日志
来源：http://giv.jiagoushi.top

split -l 1000 big.log part_
来源：http://ydi.tianlin.xyz

[R74] 批量重命名
来源：http://sgm.wangdashe.top

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pft.vehdjk.com

[R75] 导出环境变量
来源：http://pyn.jianghu66.top

export PATH="$HOME/bin:$PATH"
来源：http://ndm.iojbl.cn

[R76] 使用临时文件
来源：http://plo.gotoacloud.top

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ysx.iojbl.cn

[R77] 读取用户输入
来源：http://yil.uphjek.com

read -rp "请输入: " ans
来源：http://gjq.pengpengdd.cyou

[R78] 交互式菜单
来源：http://wbo.pengpengdd.cyou

select opt in a b c; do echo "$opt"; break; done
来源：http://teg.0kj1m.cn

[R79] 解析命令行选项
来源：http://nzt.havefunace.top

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vsg.havefunace.top

[R80] 查看脚本执行耗时
来源：http://gfr.bbcook.cn

time ./run.sh
来源：http://lrh.hesvh.cn

================================================================================
来源：http://tng.bbcook.cn

S. C / C++ 专题
来源：http://txb.haohaochexian.top

================================================================================
来源：http://ywv.xuetiantiany.cn

[S01] C：Hello World
来源：http://ayq.cdnleiting.top

#include <stdio.h>
来源：http://bjc.shzxlz.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qee.xylfe.cn

[S02] C：变量与格式化输出
来源：http://acg.yj20258.top

int a = 10; printf("%d\n", a);
来源：http://zso.hfpthk.cn

[S03] C：读入整数
来源：http://bsl.meibo888.top

int x; scanf("%d", &x);
来源：http://snb.dianchejie.cn

[S04] C：字符串复制
来源：http://esi.jinqigfzy.top

char dst[32]; strcpy(dst, "hi");
来源：http://hht.yuxming.cn

[S05] C：字符串长度
来源：http://jho.zhijiandao.cn

strlen(s)
来源：http://tgs.daxiang520.top

[S06] C：字符串比较
来源：http://lcl.andypj.xyz

strcmp(a, b) == 0
来源：http://jue.ybcxt.top

[S07] C：数组遍历求和
来源：http://cen.52xcode.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://jdu.epnwcf.com

[S08] C：动态内存分配与释放
来源：http://kxd.ctjpmb.com

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ail.xylfe.cn

[S09] C：结构体定义与初始化
来源：http://uia.sxryk.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bmm.yueranfly.top

[S10] C：指针与解引用
来源：http://mbc.jqgufenzy.top

int *p = &a;  *p = 5;
来源：http://jvh.shuidangran.top

[S11] C：逐行读文件
来源：http://ovy.jyoumei.cn

FILE *f = fopen("a.txt", "r");
来源：http://bko.hnqzz.top

while (fgets(buf, sizeof buf, f)) { }
来源：http://xsc.xinyue.icu

fclose(f);
来源：http://mqw.andypj.xyz

[S12] C：写文件
来源：http://qkd.jyoumei.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sya.dianchejie.cn

[S13] C：宏定义
来源：http://rbx.snrcjt.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sdv.sxryk.cn

[S14] C：枚举
来源：http://hqq.haohaochexian.top

enum Color { RED, GREEN, BLUE };
来源：http://epq.jinqigfzy.top

[S15] C：类型转换
来源：http://gps.yuanzhike.top

(double) a / b
来源：http://ran.epnwcf.com

[S16] C：位操作置位
来源：http://dsm.zhijiandao.cn

x |= (1 << 3);
来源：http://tpl.zhoulong.xyz

[S17] C：安全拼接字符串
来源：http://dmm.sysykeji.top

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://usc.snrcjt.cn

[S18] C：命令行参数
来源：http://dhv.zhaomingkeji.xyz

int main(int argc, char **argv)
来源：http://qvh.fanxiaobao.xyz

[S19] C：快速排序
来源：http://hso.bjfxy.top

qsort(a, n, sizeof(int), cmp);
来源：http://pah.zdbjq.cn

[S20] C：二分查找
来源：http://odc.svipenyu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://snr.aibaodan.cn

[S21] C：字符类别判断
来源：http://ade.gaohongyu789.top

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mtd.zdbjq.cn

[S22] C：字符串转数字
来源：http://xts.shzxlz.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rko.haohaochexian.top

[S23] C：随机数
来源：http://npc.fengsongda.top

srand(time(NULL));  int r = rand() % 100;
来源：http://plh.vehdjk.com

[S24] C：获取本地时间
来源：http://xll.dianchejie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://feu.gotoacloud.top

[S25] C：内存拷贝
来源：http://asd.jyoumei.cn

memcpy(dst, src, n);
来源：http://kdw.shanyushiyangkeji.top

[S26] C：内存清零
来源：http://uih.wangdashe.top

memset(a, 0, sizeof a);
来源：http://ceg.zhoulong.xyz

[S27] C：定义常量
来源：http://uiy.yanxiufei.cn

const double PI = 3.14159;
来源：http://oau.ywan-chungtsiang.top

[S28] C：静态变量
来源：http://xbn.xuanzx.com


<!-- 参考信息 -->